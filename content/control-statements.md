### 📚 **สรุปเนื้อหาเรื่อง Control Statements (ภาษาไทย พร้อมตัวอย่างโค้ด)**

---

## ✅ **if Statement**
```java
int number = 10;
if (number > 0) {
    System.out.println("The number is positive.");  // ผลลัพธ์: The number is positive.
}
```

---

## ✅ **if...else Statement**
```java
int number = -5;
if (number > 0) {
    System.out.println("The number is positive.");
} else {
    System.out.println("The number is negative.");  // ผลลัพธ์: The number is negative.
}
```

---

## ✅ **Nested if Statement**
```java
int score = 85;

if (score >= 90) {
    System.out.println("Grade: A");
} else if (score >= 80) {
    System.out.println("Grade: B");  // ผลลัพธ์: Grade: B
} else if (score >= 70) {
    System.out.println("Grade: C");
} else {
    System.out.println("Grade: F");
}
```

---

## ✅ **switch Statement**
```java
int day = 3;

switch (day) {
    case 1:
        System.out.println("Monday");
        break;
    case 2:
        System.out.println("Tuesday");
        break;
    case 3:
        System.out.println("Wednesday");  // ผลลัพธ์: Wednesday
        break;
    default:
        System.out.println("Invalid day");
}
```

---

## ✅ **while Loop**
```java
int i = 0;
while (i < 5) {
    System.out.println("Count: " + i);
    i++;
}
// ผลลัพธ์:
// Count: 0
// Count: 1
// Count: 2
// Count: 3
// Count: 4
```

---

## ✅ **do...while Loop**
```java
int i = 0;
do {
    System.out.println("Count: " + i);
    i++;
} while (i < 5);
// ผลลัพธ์เหมือนกับ while loop
```

---

## ✅ **for Loop**
```java
for (int i = 1; i <= 5; i++) {
    System.out.println("Iteration: " + i);
}
// ผลลัพธ์:
// Iteration: 1
// Iteration: 2
// Iteration: 3
// Iteration: 4
// Iteration: 5
```

---

## ✅ **Nested for Loop**
```java
for (int i = 1; i <= 2; i++) {
    for (int j = 1; j <= 4; j++) {
        System.out.print(j + " ");
    }
    System.out.println();
}
// ผลลัพธ์:
// 1 2 3 4 
// 1 2 3 4
```

---

## ✅ **break Statement**
```java
for (int i = 1; i <= 5; i++) {
    if (i == 3) {
        break;
    }
    System.out.println("Iteration: " + i);
}
// ผลลัพธ์:
// Iteration: 1
// Iteration: 2
```

---

## ✅ **continue Statement**
```java
for (int i = 1; i <= 5; i++) {
    if (i == 3) {
        continue;
    }
    System.out.println("Iteration: " + i);
}
// ผลลัพธ์:
// Iteration: 1
// Iteration: 2
// Iteration: 4
// Iteration: 5
```

---

## ✅ **การใช้ Scanner รับค่าจากผู้ใช้**
```java
import java.util.Scanner;

public class UserInput {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter your age: ");
        int age = scanner.nextInt();

        if (age >= 18) {
            System.out.println("You are an adult.");
        } else {
            System.out.println("You are not an adult.");
        }

        scanner.close();
    }
}
```

---
