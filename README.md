#include <SoftwareSerial.h>

SoftwareSerial BT(2, 3);  // RX, TX
int ledPin = 13;
char command;

void setup() {
  pinMode(ledPin, OUTPUT);
  BT.begin(9600);
  Serial.begin(9600);
  Serial.println("Bluetooth LED Control Ready");
}

void loop() {
  if (BT.available()) {
    command = BT.read();
    Serial.println(command);
    
    if (command == '1') {
      digitalWrite(ledPin, HIGH);
      Serial.println("LED ON");
    } 
    else if (command == '0') {
      digitalWrite(ledPin, LOW);
      Serial.println("LED OFF");
    }
  }
}
