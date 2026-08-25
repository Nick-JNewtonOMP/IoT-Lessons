<img width="784" height="278" alt="OMP-logo" src="https://github.com/user-attachments/assets/f615e47e-d6fa-44c3-bdd3-7a76707ea047" />







# IoT Lessons | บทเรียน IoT

---
<details>
<summary><strong>Week 1 — Introduction to IoT: LED Tree | สัปดาห์ที่ 1 — แนะนำ IoT: ต้นไม้ LED</strong></summary>
<br>
  
## Lesson 1 — Introduction to IoT | บทที่ 1 — แนะนำ IoT
In this lesson there was no code needed. | ในบทเรียนนี้ไม่จำเป็นต้องใช้โค้ด
But please feel free to check out | แต่สามารถดูข้อมูลเพิ่มเติมได้ที่
[Autodesk Instructables](https://www.instructables.com/)

---

## Lesson 2 — Hardware and software | บทที่ 2 — ฮาร์ดแวร์และซอฟต์แวร์

### 1) One Blinking LED | หนึ่ง LED กะพริบ
```cpp
// Define variables | กำหนดตัวแปร
#define LED_PIN_1 0
void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  pinMode(LED_PIN_1,OUTPUT); 
}
void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
    digitalWrite(LED_PIN_1,HIGH);
    delay(1000);
    digitalWrite(LED_PIN_1,LOW);
    delay(1000);
}
```

### 2) Multiple Blinking LEDs | หลาย LED กะพริบ
```cpp
// Define variables | กำหนดตัวแปร
#define LED_PIN_1 0
#define LED_PIN_2 25
#define LED_PIN_3 26
#define LED_PIN_4 27
void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  pinMode(LED_PIN_1,OUTPUT);
  pinMode(LED_PIN_2,OUTPUT);
  pinMode(LED_PIN_3,OUTPUT);
  pinMode(LED_PIN_4,OUTPUT);
}
void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
    digitalWrite(LED_PIN_1,HIGH);
    delay(1000);
    digitalWrite(LED_PIN_2,HIGH);
    delay(1000);
    digitalWrite(LED_PIN_3,HIGH);
    delay(1000);
    digitalWrite(LED_PIN_4,HIGH);
    delay(1000);
    digitalWrite(LED_PIN_1,LOW);
    digitalWrite(LED_PIN_2,LOW);
    digitalWrite(LED_PIN_3,LOW);
    digitalWrite(LED_PIN_4,LOW);
    delay(2000);
}
```

---

## Lesson 3 — Weekly Challenge: Christmas Tree | บทที่ 3 — ความท้าทายประจำสัปดาห์: ต้นคริสต์มาส

Please try it yourself first, and use the hints if needed. | โปรดลองทำด้วยตัวเองก่อน แล้วค่อยใช้คำใบ้หากจำเป็น

### 0) Useful Commands | คำสั่งที่มีประโยชน์
**How to use this | วิธีใช้งาน**

1. Find the code block for your task below. | หาโค้ดของงานคุณด้านล่าง
2. Click **Copy Code**. | คลิก **Copy Code**
3. Switch to **Cirkit Designer** and paste it (**Ctrl+V** or **Cmd+V**). | สลับไปที่ **Cirkit Designer** แล้ววางโค้ด (**Ctrl+V** หรือ **Cmd+V**)
 

### 1) Christmas tree no code | ไม่มีโค้ด

<details>
<summary>💡 Hint — Wiring diagram | คลิกเพื่อดูคำใบ้ — แผนผังการต่อสาย</summary>

<br>

<img width="927" height="590" alt="Christmas tree wiring diagram" src="https://github.com/user-attachments/assets/60e78ea0-661e-4d2e-94e6-64370a4918e2" />

*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*

</details>

### 2) Christmas tree with code: Blinking the top light | ต้นคริสต์มาสพร้อมโค้ด: ทำให้ไฟด้านบนกะพริบ

<details>
<summary>💡 Hint 0 — Wiring diagram | คลิกเพื่อดูคำใบ้ — แผนผังการต่อสาย</summary>
<br>
<img width="662" height="567" alt="image" src="https://github.com/user-attachments/assets/227cdb49-edae-48eb-bf94-c2b49ecb3dec" />

*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*
</details>

<details>
<summary>💡 Hint 1 — Code | คลิกเพื่อดูคำใบ้ — ดูโค้ดจากบทเรียนที่ 2</summary>
<br>
Look at code from Lesson 2: One Blinking LED. | ดูโค้ดจากบทที่ 2: LED กะพริบหนึ่งดวง
</details>

<details>
<summary>💡 Hint 2 — Code | คลิกเพื่อดูคำใบ้ — โค้ดเฉลย</summary>
<br>

```cpp
// Define variables | กำหนดตัวแปร
#define LED_PIN_1 0
void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  pinMode(LED_PIN_1,OUTPUT); 
}
void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
    digitalWrite(LED_PIN_1,HIGH);
    delay(1000);
    digitalWrite(LED_PIN_1,LOW);
    delay(1000);
}
```

</details>



### 3) Christmas tree with code: Adding decorations | ต้นคริสต์มาสพร้อมโค้ด: เพิ่มการตกแต่ง

<details>
<summary>💡 Hint 0 — Wiring diagram | คลิกเพื่อดูคำใบ้ — แผนผังการต่อสาย</summary>
<br>
<img width="758" height="597" alt="image" src="https://github.com/user-attachments/assets/514d754a-816f-4e58-9170-f3c62187fdf7" />

*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*
</details>


<details>
<summary>💡 Hint 1 — Code | คลิกเพื่อดูคำใบ้ — โค้ดเฉลย</summary>
<br>

```cpp
// Define variables | กำหนดตัวแปร
#define LED_top 0
#define LED_red_1 35
#define LED_red_2 36

void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  pinMode(LED_top,OUTPUT); 
  pinMode(LED_red_1,OUTPUT); 
  pinMode(LED_red_2,OUTPUT); 

}
void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
    digitalWrite(LED_top,HIGH);
    digitalWrite(LED_red_1,HIGH);
    digitalWrite(LED_red_2,HIGH);
    delay(1000);
    
    digitalWrite(LED_top,LOW);
    digitalWrite(LED_red_1,LOW);
    digitalWrite(LED_red_2,LOW);
    delay(1000);
}
```

</details>



### 4) Christmas tree with code: Make it yours! | ต้นคริสต์มาสพร้อมโค้ด: ทำให้เป็นของคุณเอง!

Try things and see what happens! | ลองทำแล้วดูว่าเกิดอะไรขึ้น!

<details>
<summary>🎄 Suggestion 0 — Wiring | คลิกเพื่อดูไอเดีย — การต่อสาย</summary>
<br>
Start from the wiring you already made and add something new. How about a blue LED? Or two? The circuit is yours to expand! | เริ่มจากการต่อสายที่คุณทำไว้แล้ว แล้วเพิ่มสิ่งใหม่เข้าไป เช่น LED สีน้ำเงิน หรือจะเพิ่มสองดวงก็ได้!
</details>

<details>
<summary>🎄 Suggestion 1 — Play with the order | คลิกเพื่อดูไอเดีย — ลองเปลี่ยนลำดับ</summary>
<br>
Until now the LEDs always turned on and off together. Try switching the order and mixing HIGH and LOW. What happens if one turns on while another turns off at the same time? | จนถึงตอนนี้ LED จะติดและดับพร้อมกันเสมอ ลองสลับลำดับและผสม HIGH กับ LOW ดู จะเกิดอะไรขึ้นถ้าดวงหนึ่งติดในขณะที่อีกดวงดับ?

Try something like this: | ลองแบบนี้ดู:

```cpp
void loop() {
  // Mix HIGH and LOW with delays in between | ผสม HIGH และ LOW โดยมี delay คั่นกลาง
    digitalWrite(LED_top, HIGH);
    delay(500);
    digitalWrite(LED_red_1, HIGH);
    digitalWrite(LED_red_2, LOW);
    delay(500);
    digitalWrite(LED_red_1, LOW);
    digitalWrite(LED_red_2, HIGH);
    delay(300);
    digitalWrite(LED_top, LOW);
    digitalWrite(LED_red_2, LOW);
    delay(1000);
}
```

Or try this: | หรือลองแบบนี้:

```cpp
void loop() {
  // One on, one off, one waiting | ดวงหนึ่งติด ดวงหนึ่งดับ ดวงหนึ่งรออยู่
    digitalWrite(LED_red_1, HIGH);
    delay(200);
    digitalWrite(LED_red_2, LOW);
    delay(200);
    digitalWrite(LED_red_1, LOW);
    delay(200);
    digitalWrite(LED_red_2, HIGH);
    delay(500);
}
```

Or try this: | หรือลองแบบนี้:

```cpp
  
void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
    digitalWrite(LED_top,HIGH);
    delay(1000);
    digitalWrite(LED_red_1,HIGH);
    delay(2000);
    digitalWrite(LED_red_2,HIGH);
    delay(3000);
    
    digitalWrite(LED_top,LOW);
    delay(1000);
    digitalWrite(LED_red_1,LOW);
    delay(2000);
    digitalWrite(LED_red_2,LOW);
    delay(500);
}
```
</details>

<details>
<summary>🎄 Suggestion 2 — Take full control | คลิกเพื่อดูไอเดีย — ควบคุม LED ทั้งหมด</summary>
<br>
Can you control every single LED on the tree? Give each one its own timing and mix HIGH and LOW however you like. Just keep an eye on which pins you are using on the ESP32! | ลองควบคุม LED ทุกดวงบนต้นไม้ได้เลย ให้แต่ละดวงมีจังหวะเป็นของตัวเอง แค่ระวังขาพินที่ใช้บน ESP32 ด้วย! 
</details>

</details>



<details>
<summary><strong>Week 2 — Resistors, Sensors and Input | สัปดาห์ที่ 2 — เซ็นเซอร์ หน้าจอ และข้อมูล</strong></summary>
<br>

## Lesson 1 — Resistors and Circuits | บทที่ 1 — ตัวต้านทานและวงจร

Please try it yourself first, and use the hints if needed. | โปรดลองทำด้วยตัวเองก่อน แล้วค่อยใช้คำใบ้หากจำเป็น


 ---

### 1)  What happens when you change the resistor value? | เกิดอะไรขึ้นเมื่อคุณเปลี่ยนค่าตัวต้านทาน?
 

<details>
<summary>🔌 Wiring diagram | คลิกเพื่อดูแผนผังการต่อสาย </summary>

Wire your circuit as shown in the figure below. | ต่อวงจรตามภาพด้านล่าง

**Components | อุปกรณ์:** Resistor, LED, 5V DC Power Supply, 7-Segment Panel Voltmeter | ตัวต้านทาน, LED, แหล่งจ่ายไฟ 5V, โวลต์มิเตอร์

The Voltmeter lets you measure the voltage across your components in your circuit as you change the resistor value. Also pay attention to the brightness of the LED. It tells you a lot! | โวลต์มิเตอร์ช่วยให้คุณวัดแรงดันไฟฟ้าที่คร่อมอุปกรณ์แต่ละชิ้นขณะที่เปลี่ยนค่าตัวต้านทาน และสังเกตความสว่างของ LED ด้วย มันบอกอะไรคุณได้มาก!

🤔 Think about it | ลองคิดดู:
- What happens when you **increase** the resistance? | เกิดอะไรขึ้นเมื่อ**เพิ่ม**ค่าความต้านทาน?
- What happens when you **decrease** the resistance? | เกิดอะไรขึ้นเมื่อ**ลด**ค่าความต้านทาน?

<br>

<img width="812" height="672" alt="image" src="https://github.com/user-attachments/assets/67e00d46-76dd-463b-a5f1-5bdd8efc8fb3" />


*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*

</details>



### 2)  Series circuit | วงจรอนุกรม

<details>
<summary>🔌 Wiring diagram | คลิกเพื่อดูแผนผังการต่อสาย </summary>

Build the circuit shown below. | สร้างวงจรตามภาพด้านล่าง

**Components | อุปกรณ์:** Resistors, LEDs, 5V DC Power Supply, Switch | ตัวต้านทาน, LED, แหล่งจ่ายไฟ 5V, สวิตช์

The top diagram shows a series circuit where all components are connected in one single loop. What happens to the brightness of the LEDs when you change the resistor value? | แผนผังด้านบนแสดงวงจรอนุกรมที่อุปกรณ์ทั้งหมดต่อกันเป็นวงเดียว เกิดอะไรขึ้นกับความสว่างของ LED เมื่อคุณเปลี่ยนค่าตัวต้านทาน?

🤔 Now try this | ลองสิ่งนี้:

What happens when you remove one LED from a series circuit? In a real circuit you would cut the wire. Here you can simulate that using the switch at the bottom. An **open switch** means the wire is cut. | จะเกิดอะไรขึ้นเมื่อถอด LED ออกหนึ่งดวงจากวงจรอนุกรม? ในวงจรจริงคุณจะต้องตัดสาย แต่ที่นี่คุณสามารถจำลองได้โดยใช้สวิตช์ **สวิตช์เปิด** หมายความว่าสายถูกตัด

<br>
<img width="383" height="583" alt="image" src="https://github.com/user-attachments/assets/c7750214-ef10-4de1-8ff1-dd253cc9340b" />


*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*

</details>


### 3) Parallel circuit | วงจรขนาน

<details>
<summary>🔌 Wiring diagram | คลิกเพื่อดูแผนผังการต่อสาย</summary>
<br>

Build the circuit shown below. | สร้างวงจรตามภาพด้านล่าง

**Components | อุปกรณ์:** Resistors, LEDs, 5V DC Power Supply, Switch | ตัวต้านทาน, LED, แหล่งจ่ายไฟ 5V, สวิตช์

The top diagram shows a parallel circuit where components are connected across two separate loops. What happens to the brightness of the LEDs when you change the resistor values? Try keeping one resistor value constant while increasing or decreasing the other one. Do both LEDs behave the same way? | แผนผังด้านบนแสดงวงจรขนานที่อุปกรณ์ต่อกันในสองวงแยกกัน เกิดอะไรขึ้นกับความสว่างของ LED เมื่อคุณเปลี่ยนค่าตัวต้านทาน? ลองเก็บค่าตัวต้านทานตัวหนึ่งไว้คงที่แล้วเพิ่มหรือลดอีกตัวหนึ่ง LED ทั้งสองดวงมีพฤติกรรมเหมือนกันไหม?

🤔 Now try this | ลองสิ่งนี้:

What happens when you remove one LED from a parallel circuit? In a real circuit you would cut the wire. Here you can simulate that using the switch at the bottom. An **open switch** means the wire is cut. Does the other LED stay on? | จะเกิดอะไรขึ้นเมื่อถอด LED ออกหนึ่งดวงจากวงจรขนาน? ในวงจรจริงคุณจะต้องตัดสาย แต่ที่นี่คุณสามารถจำลองได้โดยใช้สวิตช์ **สวิตช์เปิด** หมายความว่าสายถูกตัด LED อีกดวงยังติดอยู่ไหม?

<br>
<img width="487" height="595" alt="image" src="https://github.com/user-attachments/assets/6352448f-fe66-40da-9102-e3adc587ac0f" />

*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*

</details>

### 4) LDR | เซ็นเซอร์แสง LDR

<details>
<summary>🔌 Wiring diagram | คลิกเพื่อดูแผนผังการต่อสาย</summary>
<br>

Build the circuit shown below. | สร้างวงจรตามภาพด้านล่าง

**Components | อุปกรณ์:** LDR, ESP32 | LDR (ตัวต้านทานแสง), ESP32

Connect the VCC pin of the LDR to the positive rail. Connect the GND pin of the LDR to the negative rail. Connect the A0 pin to pin 2 of the ESP32 board. | ต่อขา VCC ของ LDR เข้ากับราง positive ต่อขา GND ของ LDR เข้ากับราง negative และต่อขา A0 เข้ากับขา 2 ของบอร์ด ESP32 

<br>

<img width="656" height="471" alt="image" src="https://github.com/user-attachments/assets/d270a7d0-5009-4a14-a3cd-04871e883500" />


*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*

</details>



<details>
<summary>💡 Hint 1 — Define your pin | คลิกเพื่อดูคำใบ้ — กำหนดขาพิน</summary>
<br>

Do you remember to define and name your pin using **define** ? | คุณจำได้ไหมว่าต้องกำหนดและตั้งชื่อขาพินโดยใช้ **define** อย่างไร?
```cpp
// Define variables | กำหนดตัวแปร
  #define LDR_Pin 2 
```

</details>


<details>
<summary>💡 Hint 2 — Setup | คลิกเพื่อดูคำใบ้ — การตั้งค่าเริ่มต้น</summary>
<br>

Start with the setup. We need to define the pin function and start the Serial Monitor. Do you remember the **pinMode** function? This time the pin is an INPUT not an OUTPUT. | เริ่มด้วยการตั้งค่า เราต้องกำหนดฟังก์ชันของขาพินและเริ่มต้น Serial Monitor คุณจำฟังก์ชัน **pinMode** ได้ไหม? คราวนี้ขาพินเป็น INPUT ไม่ใช่ OUTPUT

```cpp
// Define variables | กำหนดตัวแปร
#define LDR_Pin 2

void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
    Serial.begin(9600);
    pinMode(LDR_Pin,INPUT);
}

```

</details>

<details>
<summary>💡 Hint 3 — Loop | คลิกเพื่อดูคำใบ้ — การวนซ้ำ</summary>
<br>
  
Next is the loop. We need to read the incoming data from the LDR and show it in the Serial Monitor. | ตอนนี้เขียนส่วน loop เราต้องอ่านข้อมูลที่เข้ามาจาก LDR และแสดงผลใน Serial Monitor

Here is what each line does | แต่ละบรรทัดทำหน้าที่ดังนี้:

- **int** tells the code what type of data to expect. In this case integer numbers. | **int** บอกโค้ดว่าข้อมูลที่ได้รับเป็นชนิดใด ในที่นี้คือจำนวนเต็ม
- **LDR_value** is the name we give to that data. | **LDR_value** คือชื่อที่เราตั้งให้กับข้อมูลนั้น
- **analogRead** reads the value coming from the pin. | **analogRead** อ่านค่าที่มาจากขาพิน
- **Serial.println** shows the value in the Serial Monitor. We use **println** and not **print** so each new value appears on a new line. | **Serial.println** แสดงค่าใน Serial Monitor เราใช้ **println** ไม่ใช่ **print** เพื่อให้ค่าใหม่แต่ละค่าแสดงบนบรรทัดใหม่
- **delay** gives the microcontroller time to process. Without it the Serial Monitor gets flooded with data and may freeze. | **delay** ให้เวลาไมโครคอนโทรลเลอร์ประมวลผล หากไม่มี delay Serial Monitor จะรับข้อมูลมากเกินไปและอาจค้าง

- 🤔 Try it yourself: swap Serial.println() for Serial.print() and see what changes in the Serial Monitor. | ลองด้วยตัวเอง: เปลี่ยน Serial.println() เป็น Serial.print() แล้วดูว่าเกิดอะไรขึ้นใน Serial Monitor

```cpp
// Define variables | กำหนดตัวแปร
#define LDR_Pin 2

void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  Serial.begin(9600);
  pinMode(LDR_Pin, INPUT);
}

void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
  int LDR_value = analogRead(LDR_Pin);
  Serial.println(LDR_value);
  delay(500);
}
```

</details>


<details>
<summary>💡 Hint 4 — Complete Code | คลิกเพื่อดูโค้ดทั้งหมด</summary>
<br>
  

```cpp
// Define variables | กำหนดตัวแปร
#define LDR_Pin 2

void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  Serial.begin(9600);
  pinMode(LDR_Pin, INPUT);
}

void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
  int LDR_value = analogRead(LDR_Pin);
  Serial.println(LDR_value);
  delay(500);
}
```

</details>

---

## Lesson 2 — Pins, Conditions and Sensors | บทที่ 2 — พิน เงื่อนไข และเซ็นเซอร์

Please try it yourself first, and use the hints if needed. | โปรดลองทำด้วยตัวเองก่อน แล้วค่อยใช้คำใบ้หากจำเป็น


 ---
### 1)  LED Blinks when the room is dark | LED กะพริบเมื่อห้องมืด

Your challenge: when a room goes dark let an LED blink and warn the user by printing a message to the Serial Monitor. Use the LDR diagram from yesterday (Lesson 4). Which pin should you use? Do you need an accurate measurement or just an on or off signal? | ความท้าทายของคุณ: เมื่อห้องมืดลง ให้ LED กะพริบและแจ้งเตือนผู้ใช้โดยพิมพ์ข้อความไปยัง Serial Monitor ใช้แผนผังการต่อสาย LDR จากเมื่อวาน (บทที่ 4) คุณควรใช้ขาพินใด? คุณต้องการการวัดที่แม่นยำหรือแค่สัญญาณเปิดหรือปิด?

<details>
<summary>🔌 Wiring diagram | คลิกเพื่อดูแผนผังการต่อสาย </summary>

Wire your circuit as shown in the figure below. | ต่อวงจรตามภาพด้านล่าง

**Components | อุปกรณ์:** LDR, ESP32, LED, Resistor | LDR (ตัวต้านทานแสง), ESP32, LED, Resistor


<br>

<img width="497" height="422" alt="image" src="https://github.com/user-attachments/assets/c1e09d0a-64af-4c60-9fbd-1251a001747c" />


*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*

</details>


<details>
<summary>💡 Hint 1 — Digital or Analogue |คลิกเพื่อดูคำใบ้ — ดิจิทัลหรืออนาล็อก</summary>
<br>

Since we only want to know when the room is dark or not, the digital pin is sufficient. | เนื่องจากเราต้องการรู้เพียงว่าห้องมืดหรือไม่ ขาดิจิทัลก็เพียงพอแล้ว
```cpp
// Define variables | กำหนดตัวแปร
#define LED_Pin 0
#define LDR_Digital 8

```
</details>


<details>
<summary>💡 Hint 2 — Setup | คลิกเพื่อดูคำใบ้ — การตั้งค่าเริ่มต้น</summary>
<br>

Which pin is **INPUT** and which one is **OUTPUT**?

```cpp
void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  Serial.begin(9600);
  pinMode(LDR_Digital, INPUT);
  pinMode(LED_Pin,OUTPUT);
}

```
</details>


<details>
<summary>💡 Hint 3 — Loop | vคลิกเพื่อดูคำใบ้ — การวนซ้ำ</summary>
<br>

Which statement do you need? How many conditions are there?

```cpp
void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
    int LDR_Threshold = digitalRead(LDR_Digital);
    if (LDR_Threshold == HIGH){
        Serial.println("ROOM IS DARK!");
        Serial.println("Switching on LED");
        digitalWrite(LED_Pin,HIGH);
        delay(500);
        digitalWrite(LED_Pin,LOW);
        delay(500);
    }

    else{
        digitalWrite(LED_Pin,LOW);
        delay(100);
    }
}


```
</details>


### 2)  Add the analogue value | เพิ่มค่าอนาล็อก


Use the same circuit as above but now also show the LDR values on the Serial Monitor when the room is dark. | ใช้วงจรเดิมจากข้างบน แต่คราวนี้ให้แสดงค่าแสงบน Serial Monitor ด้วยเมื่อห้องมืด

🤔 Think about it: you already have the digital pin telling you when it is dark. Now you just need to add the analogue pin to measure how dark it actually is. | ลองคิดดู: คุณมีขาดิจิทัลที่บอกว่าห้องมืดแล้ว ตอนนี้แค่เพิ่มขาอนาล็อกเพื่อวัดว่ามืดแค่ไหน


<details>
<summary>💡 Hint 1 — Add the analogue pin | คลิกเพื่อดูคำใบ้ — เพิ่มขาอนาล็อก</summary>
<br>

Add a new pin definition for the analogue LDR pin. | เพิ่มการกำหนดขาพินใหม่สำหรับขาอนาล็อกของ LDR

```cpp
// Define variables | กำหนดตัวแปร
#define LED_Pin 0
#define LDR_Digital 8
#define LDR_Analogue 2

```

</details>

<details>
<summary>💡 Hint 2 — Setup |  คลิกเพื่อดูคำใบ้ — การตั้งค่าเริ่มต้น</summary>
<br>

Add **pinMode(LDR_Analogue,INPUT);** to the Setup function. Note the INPUT and not OUTPUT. | เพิ่ม **pinMode(LDR_Analogue,INPUT);** ในฟังก์ชัน setup. โปรดสังเกตว่าเป็น INPUT ไม่ใช่ OUTPUT

</details>


<details>
<summary>💡 Hint 3 — loop | คลิกเพื่อดูคำใบ้ — การวนซ้ำ</summary>
<br>

Remember | จำไว้ว่า:
- Read the analogue value using **analogRead(LDR_Analogue)** | อ่านค่าอนาล็อกโดยใช้ **analogRead(LDR_Analogue)**
- Show it on the Serial Monitor using **Serial.println()** | แสดงผลบน Serial Monitor โดยใช้ **Serial.println()**


```cpp
int LDR_Value = analogRead(LDR_Analogue);
```

</details>

<details>
<summary>💡 Hint 4 — Full solution | คลิกเพื่อดูโค้ดทั้งหมด </summary>
<br>


```cpp
// Define variables | กำหนดตัวแปร
#define LED_Pin 0
#define LDR_Digital 8
#define LDR_Analogue 2

void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  Serial.begin(9600);
  pinMode(LDR_Analogue, INPUT);
  pinMode(LDR_Digital, INPUT);
  pinMode(LED_Pin,OUTPUT);
}

void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
    int LDR_Value = analogRead(LDR_Analogue);
    int LDR_Threshold = digitalRead(LDR_Digital);

    if (LDR_Threshold == HIGH){
        Serial.println("ROOM IS DARK!");
        Serial.println("Switching on LED");

        Serial.println(LDR_Value);
        digitalWrite(LED_Pin,HIGH);
        delay(500);
        digitalWrite(LED_Pin,LOW);
        delay(500);

    }

    else{
        digitalWrite(LED_Pin,LOW);
        delay(100);
    }
}


```

</details>


### 3)  What is wrong? | มีอะไรผิดพลาด?

Your challenge: why does the following setup not work? What is the mistake in the code and what is the mistake in the wiring? | ความท้าทายของคุณ: ทำไมการตั้งค่าต่อไปนี้ถึงไม่ทำงาน? มีข้อผิดพลาดอะไรในโค้ด และมีข้อผิดพลาดอะไรในการต่อสาย?


<details>
<summary>🔌 Wiring diagram | คลิกเพื่อดูแผนผังการต่อสาย </summary>

Wire your circuit as shown in the figure below. | ต่อวงจรตามภาพด้านล่าง

**Components | อุปกรณ์:** LDR, ESP32, LED, Resistor | LDR (ตัวต้านทานแสง), ESP32, LED, Resistor


<br>

<img width="655" height="446" alt="image" src="https://github.com/user-attachments/assets/740ab63e-49e2-4077-bb71-652777784668" />


*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*

</details>


<details>
<summary>🔌 Code | คลิกเพื่อดูโค้ด </summary>
  
Can you spot the mistakes and fix them? | คุณสามารถหาข้อผิดพลาดและแก้ไขได้ไหม?


<br>

```cpp
// Define variables | กำหนดตัวแปร
#define LED_Pin 0
#define LDR_Digital 8
#define LDR_Analogue 2

void setup() {
  // Put your setup code here, to run once: | ใส่โค้ดตั้งค่าที่นี่ รันครั้งเดียว
  Serial.begin(9600);
  pinMode(LDR_Analogue, INPUT);

  pinMode(LDR_Digital, OUTPUT);
  pinMode(LED_Pin,OUTPUT);
}

void loop() {
  // Put your main code here, to run repeatedly: | ใส่โค้ดหลักที่นี่ รันซ้ำๆ
    int LDR_Value = analogRead(LDR_Pin);
    int LDR_Threshold = digitalRead(LDR_Digital);

    if (LDR_Threshold == HIGH){
        Serial.println("ROOM IS DARK!");
        Serial.print("Switching on LED");

        Serial.println(LDR_Value);
        digitalWrite(LED_Pin,HIGH)
        delay(500);
        digitalWrite(LED_Pin,LOW);
        delay(500);

    }

    else{
        digitalWrite(LED_Pin,HIGH);
        delay(100);
    }


}


```

</details>



### 4) Try a different sensor: Flame sensor! | ลองใช้เซ็นเซอร์ต่างชนิด: เซ็นเซอร์เปลวไฟ!

Your challenge: you have a new sensor. Can you work out how to wire it and write the code yourself? Look at the sensor carefully: does it remind you of anything you have used before? | ความท้าทายของคุณ: คุณมีเซ็นเซอร์ใหม่ คุณสามารถคิดวิธีต่อสายและเขียนโค้ดเองได้ไหม? สังเกตเซ็นเซอร์ดีๆ มันทำให้คุณนึกถึงอะไรที่เคยใช้มาก่อนไหม?


<details>
<summary>💡 Hint 1 — Stuck on the wiring? | คลิกเพื่อดูคำใบ้ — ติดปัญหาเรื่องการต่อสาย?</summary>
<br>
  
Does this module look familiar? G = GND and + = VCC. | โมดูลนี้ดูคุ้นเคยไหม? G = GND และ + = VCC

<img width="720" height="391" alt="image" src="https://github.com/user-attachments/assets/b55e6bbf-3738-4666-b2a1-289d750e6870" />

*Image made with [Cirkit Designer](https://app.cirkitdesigner.com/) | ภาพสร้างด้วย Cirkit Designer*

</details>


<details>
<summary>💡 Hint 2 — Stuck on the code? | คลิกเพื่อดูคำใบ้ — ติดปัญหาเรื่องโค้ด?</summary>

What type of signal do I want to receive? Simple ON/OFF or specific values? Does this remind you of something? Light or no light? | ฉันต้องการรับสัญญาณแบบใด? แบบเปิด/ปิด หรือค่าที่เฉพาะเจาะจง? สิ่งนี้ทำให้คุณนึกถึงอะไรไหม? มีแสงหรือไม่มีแสง?


</details>

### 5) Finished everything? Keep exploring! | เสร็จทุกอย่างแล้ว? ลองสำรวจต่อไป!

You have now worked with some sensors. Pick any sensor from the box and try to get it working on your own. Use what you have learned and see how far you can get! | ตอนนี้คุณได้ทดลองใช้เซ็นเซอร์บางตัวแล้ว เลือกเซ็นเซอร์ใดก็ได้จากกล่องแล้วลองทำให้มันทำงานด้วยตัวเอง ใช้สิ่งที่คุณได้เรียนรู้และดูว่าคุณไปได้ไกลแค่ไหน!


---


</details>
