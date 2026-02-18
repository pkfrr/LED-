// Analog Pin อ่านค่า Variable Resistor
const int potPin = A0;

// Digital PWM Pin ควบคุม LED
const int ledPin = 11;

void setup() {
  // ตั้งค่า ledPin เป็น Output
  pinMode(ledPin, OUTPUT);
}

void loop() {
  // อ่านค่า Potentiometer (0-1023) แปลงเป็น 0-255 ส่งให้ LED
  int brightness = map(analogRead(potPin), 0, 1023, 0, 255);
  
  // ส่งค่าความสว่างไปให้ LED
  analogWrite(ledPin, brightness);
  
  // หน่วงเวลา 100 มิลลิวินาที
  delay(100);
}

<iframe name="xxx" width="100%" height="100%" frameborder="0" src="homeN.html"></iframe>

<a href="homeN1.html" target="xxx">หน้าหลัก</a>




