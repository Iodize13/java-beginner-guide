### 📚 **สรุปเนื้อหาเรื่อง Methods (ภาษาไทย พร้อมตัวอย่างโค้ด)**

---

## ✅ **ตัวอย่างโครงสร้าง Method พื้นฐาน**
```java
public class MethodsExample {
    // Method ชื่อ add รับพารามิเตอร์สองตัวและคืนค่าผลรวม
    public static int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int result = add(5, 10);
        System.out.println("Result: " + result);  // ผลลัพธ์: 15
    }
}
```

---

## ✅ **ตัวอย่างการประกาศและนิยาม Method**
```java
// การประกาศ Method
static int max(int num1, int num2);

// การนิยาม Method
static int max(int num1, int num2) {
    if (num1 > num2) {
        return num1;
    } else {
        return num2;
    }
}
```

---

## ✅ **การเรียกใช้งาน Method (Method Call)**
```java
public static void main(String[] args) {
    int i = 5;
    int j = 2;
    int result = max(i, j);
    System.out.println("Max value is: " + result);  // ผลลัพธ์: Max value is: 5
}
```

---

## ✅ **การส่งค่าพารามิเตอร์ (Passing Parameters)**
```java
// Method สลับค่าตัวแปรสองตัว
static void swap(int a, int b) {
    int temp = a;
    a = b;
    b = temp;
    System.out.println("Inside swap method: a = " + a + ", b = " + b);
}

public static void main(String[] args) {
    int m = 2;
    int n = 3;
    System.out.println("Before swap: m = " + m + ", n = " + n);
    swap(m, n);
    System.out.println("After swap: m = " + m + ", n = " + n);  // ค่าไม่เปลี่ยน
}
```

---

## ✅ **การ Overloading Method**
```java
// การ Overloading Method ด้วยชื่อเดียวกันแต่ต่างกันที่ชนิดพารามิเตอร์
static int max(int num1, int num2) {
    return (num1 > num2) ? num1 : num2;
}

static double max(double num1, double num2) {
    return (num1 > num2) ? num1 : num2;
}

public static void main(String[] args) {
    System.out.println(max(5, 10));        // ผลลัพธ์: 10
    System.out.println(max(5.5, 10.1));    // ผลลัพธ์: 10.1
}
```

---

## ✅ **Method ที่เรียกตัวเอง (Recursive Method)**
```java
// การคำนวณ Factorial ด้วยการใช้ Recursive Method
static long factorial(int n) {
    if (n == 0) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}

public static void main(String[] args) {
    int number = 5;
    System.out.println("Factorial of " + number + " is " + factorial(number));  // ผลลัพธ์: 120
}
```

---

## ✅ **การใช้งาน Method จากแพ็กเกจมาตรฐาน (API)**
```java
import java.util.Scanner;

public class InputExample {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int number = input.nextInt();
        System.out.println("You entered: " + number);
        input.close();
    }
}
```

