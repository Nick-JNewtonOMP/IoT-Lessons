# IOT Lessons

---

## Lesson 1 — Introduction to IoT
In this lesson there was no code needed.
But please feel free to check out 
[Autodesk Instructables](https://www.instructables.com/)

---

## Lesson 2 — Hardware and software

### 1) One Blinking LED

```cpp

// Define variables
#define LED_PIN_1 0

void setup() {
  // Put your setup code here, to run once:
  pinMode(LED_PIN_1,OUTPUT); 
}

void loop() {
  // Put your main code here, to run repeatedly:
    digitalWrite(LED_PIN_1,HIGH);
    delay(1000);
    digitalWrite(LED_PIN_1,LOW);
    delay(1000);

}
```
### 1) Multiple Blinking LEDs

```cpp

// Define variables
#define LED_PIN_1 0
#define LED_PIN_2 25
#define LED_PIN_3 26
#define LED_PIN_4 27

void setup() {
  // Put your setup code here, to run once:
  pinMode(LED_PIN_1,OUTPUT);
  pinMode(LED_PIN_2,OUTPUT);
  pinMode(LED_PIN_3,OUTPUT);
  pinMode(LED_PIN_4,OUTPUT);
  
  
}

void loop() {
  // Put your main code here, to run repeatedly:
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


```
