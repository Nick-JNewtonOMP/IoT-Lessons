# IOT Lessons

---

## Lesson 1 — LED Basics

### 1) LED Blink

```cpp
void setup() {
  pinMode(13, OUTPUT);
}

void loop() {
  digitalWrite(13, HIGH);
  delay(1000);
  digitalWrite(13, LOW);
  delay(1000);
}
```

### 2) LED with Button

```cpp
void setup() {
  pinMode(13, OUTPUT);
  pinMode(2, INPUT_PULLUP);
}
```

---

## Lesson 2 — Sensors

### 1) Read temperature

```cpp
// your code here
```
