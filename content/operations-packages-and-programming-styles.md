### 📚 **สรุปเนื้อหาเรื่อง Operations, Packages, and Programming Styles (ภาษาไทย พร้อมตัวอย่างโค้ด)**

---

## 📌 **1. การดำเนินการทางคณิตศาสตร์ใน Java (Arithmetic Operations)**
### ✅ **ตัวอย่างการใช้งานตัวดำเนินการพื้นฐาน**
```java
int a = 10;
int b = 3;

System.out.println(a + b);   // ผลลัพธ์: 13
System.out.println(a - b);   // ผลลัพธ์: 7
System.out.println(a * b);   // ผลลัพธ์: 30
System.out.println(a / b);   // ผลลัพธ์: 3
System.out.println(a % b);   // ผลลัพธ์: 1
```

---

## 📌 **2. ตัวดำเนินการแบบย่อ (Shortcut Operators)**
```java
int num = 5;

num += 3;  // num = num + 3;
System.out.println(num);  // ผลลัพธ์: 8

num *= 2;  // num = num * 2;
System.out.println(num);  // ผลลัพธ์: 16
```

---

## 📌 **3. การเพิ่มและลดค่า (Increment & Decrement Operators)**
```java
int x = 1;

// Post-Increment (x++ ใช้ค่าเดิมก่อนค่อยเพิ่ม)
System.out.println(x++);  // ผลลัพธ์: 1
System.out.println(x);    // ผลลัพธ์: 2

// Pre-Increment (++x เพิ่มค่าก่อนแล้วค่อยใช้)
System.out.println(++x);  // ผลลัพธ์: 3
```

---

## 📌 **4. ตัวดำเนินการเปรียบเทียบ (Relational Operators)**
```java
int a = 10;
int b = 5;

System.out.println(a == b);   // ผลลัพธ์: false
System.out.println(a != b);   // ผลลัพธ์: true
System.out.println(a > b);    // ผลลัพธ์: true
System.out.println(a <= b);   // ผลลัพธ์: false
```

---

## 📌 **5. ตัวดำเนินการแบบเงื่อนไข (Conditional Operator)**
```java
int n = 3;
int next = (n % 2 == 0) ? (n / 2) : (3 * n + 1);
System.out.println(next);  // ผลลัพธ์: 10
```

---

## 📌 **6. การแปลงชนิดข้อมูล (Type Casting)**
```java
int a = 10;
double b = a;  // แปลงจาก int เป็น double อัตโนมัติ

double c = 9.99;
int d = (int) c;  // แปลงจาก double เป็น int โดยใช้การ cast
System.out.println(d);  // ผลลัพธ์: 9
```

---

## 📌 **7. การใช้แพ็กเกจใน Java (Java Packages)**
### ✅ **ตัวอย่างการนำเข้าแพ็กเกจ**
```java
import java.util.Scanner;

public class InputExample {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Enter your name: ");
        String name = input.nextLine();
        System.out.println("Hello, " + name);
        input.close();
    }
}
```

---

## 📌 **8. การจัดการเอกสารโค้ดด้วย Javadoc**
### ✅ **ตัวอย่าง Javadoc Comment**
```java
/**
 * This class demonstrates how to use Javadoc.
 * @author Oh
 * @version 1.0
 */
public class JavadocExample {

    /**
     * This method adds two numbers.
     * @param a the first number
     * @param b the second number
     * @return the sum of a and b
     */
    public static int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        System.out.println("Sum: " + add(5, 10));
    }
}
```

---
