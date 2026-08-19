<img width="784" height="278" alt="OMP-logo" src="https://github.com/user-attachments/assets/f615e47e-d6fa-44c3-bdd3-7a76707ea047" />







# IOT Lessons | บทเรียน IOT

---

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




