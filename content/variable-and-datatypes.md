### 📚 **สรุปเนื้อหาเรื่อง Variables and Data Types (Java) สำหรับเตรียมสอบ (ภาษาไทย)**

---

## 📌 **1. การเขียนโปรแกรม Java เบื้องต้น**
- **Class (คลาส)**: โครงสร้างพื้นฐานของโปรแกรม Java ทุกโปรแกรมจะต้องเริ่มต้นด้วยคลาส
- **Main Method (เมธอดหลัก)**: จุดเริ่มต้นของการทำงานในโปรแกรม Java
  ```java
  public class HelloWorld {
      public static void main(String[] args) {
          System.out.println("Hello World!");
      }
  }
  ```

---

## 📌 **2. ตัวแปร (Variables)**
- **ตัวแปร** คือ กล่องที่ใช้เก็บข้อมูลในหน่วยความจำ
- การประกาศตัวแปรใน Java ต้องระบุ **ชนิดข้อมูล (Type)** ก่อนเสมอ เช่น `int`, `double`, `String`
  ```java
  int age = 25;
  double salary = 50000.0;
  ```

---

## 📌 **3. ชนิดข้อมูลพื้นฐาน (Primitive Data Types)**
| **ชนิดข้อมูล** | **ขนาด (บิต)** | **คำอธิบาย**                  |
|----------------|-----------------|--------------------------------|
| `byte`         | 8               | จำนวนเต็มขนาดเล็ก              |
| `short`        | 16              | จำนวนเต็มขนาดกลาง              |
| `int`          | 32              | จำนวนเต็มค่าเริ่มต้น           |
| `long`         | 64              | จำนวนเต็มขนาดใหญ่              |
| `float`        | 32              | จำนวนทศนิยม                    |
| `double`       | 64              | จำนวนทศนิยมที่มีความแม่นยำสูง |
| `char`         | 16              | ตัวอักษร Unicode               |
| `boolean`      | 1               | ค่าจริงหรือเท็จ (`true/false`) |

---

## 📌 **4. นิพจน์และการกำหนดค่าให้ตัวแปร (Expressions & Variable Assignment)**
- การกำหนดค่าให้ตัวแปรใช้เครื่องหมาย `=`
  ```java
  int x = 10;
  double interest = principal * rate;
  ```

---

## 📌 **5. เมธอด (Subroutines) และแนวคิด Black-Box**
- **Subroutine** คือ ชุดคำสั่งที่รวบรวมไว้ภายใต้ชื่อเดียว และสามารถเรียกใช้ซ้ำได้
- แนวคิด **Black-Box** คือ การใช้เมธอดโดยไม่ต้องรู้รายละเอียดภายใน
  ```java
  public static int add(int a, int b) {
      return a + b;
  }
  ```

---

## 📌 **6. สายอักขระ (Strings)**
- **String** คือ ลำดับของตัวอักษร ซึ่งจัดการโดยคลาส `String`
- **เมธอดที่ใช้บ่อย**:
  - `length()`: คืนค่าความยาวของสายอักขระ
  - `charAt(index)`: คืนค่าตัวอักษรที่ตำแหน่งที่ระบุ
  - `toUpperCase()`, `toLowerCase()`: แปลงสายอักขระเป็นตัวพิมพ์ใหญ่หรือตัวพิมพ์เล็ก

---

## 📌 **7. การใช้ Enum (Enumerations)**
- **Enum** คือ ชนิดข้อมูลที่มีค่าคงที่ที่กำหนดไว้ล่วงหน้า
  ```java
  enum Season { SPRING, SUMMER, FALL, WINTER }
  Season vacation = Season.SUMMER;
  ```
- **เมธอด `ordinal()`**: ใช้คืนค่าลำดับของค่าใน Enum
  ```java
  System.out.println(Season.SUMMER.ordinal()); // ผลลัพธ์: 1
  ```

---

## 📌 **8. กฎการตั้งชื่อใน Java (Syntax Rules)**
- **Identifiers (ตัวระบุ)** คือ ชื่อที่ใช้เรียกตัวแปร คลาส หรือเมธอด
- ต้องเริ่มต้นด้วยตัวอักษรหรือ `_` และไม่มีช่องว่างระหว่างชื่อ
- ตัวพิมพ์ใหญ่และตัวพิมพ์เล็กถือว่าแตกต่างกัน เช่น `HelloWorld` ไม่เหมือนกับ `helloworld`
- ห้ามใช้ **Reserved Words (คำสงวน)** เช่น `class`, `public`, `static`, `if`, `else`

---

## 📌 **9. โครงสร้างโปรแกรม Java**
- โครงสร้างพื้นฐานของโปรแกรม Java:
  ```java
  public class ProgramName {
      public static void main(String[] args) {
          // คำสั่งที่ต้องการให้โปรแกรมทำงาน
      }
  }
  ```
- ชื่อคลาสต้องตรงกับชื่อไฟล์ เช่น คลาส `HelloWorld` ต้องบันทึกในไฟล์ `HelloWorld.java`

---

## 📌 **10. ชนิดข้อมูล Math และเมธอดที่สำคัญ**
- คลาส **Math** มีเมธอดที่ใช้คำนวณต่างๆ เช่น
  - `Math.abs(x)`: ค่าสัมบูรณ์
  - `Math.pow(x, y)`: ยกกำลัง
  - `Math.random()`: สุ่มตัวเลขระหว่าง 0 ถึง 1

---

## 📌 **11. การวัดเวลาในโปรแกรม**
- ใช้เมธอด `System.currentTimeMillis()` เพื่อวัดเวลาปัจจุบันในหน่วยมิลลิวินาที
- สามารถนำไปใช้วัดเวลาการทำงานของโปรแกรมได้
  ```java
  long startTime = System.currentTimeMillis();
  // โค้ดที่ต้องการวัดเวลา
  long endTime = System.currentTimeMillis();
  System.out.println("Run time: " + (endTime - startTime) + " ms");
  ```

---

## 📌 **12. การรับค่า Program Arguments**
- โปรแกรม Java สามารถรับค่า argument จากคอมมานด์ไลน์ได้
  ```java
  public static void main(String[] args) {
      System.out.println(args[0]); // แสดงค่า argument ตัวแรก
  }
  ```
- ใช้ `Integer.parseInt()` หรือ `Double.parseDouble()` เพื่อแปลงค่าจาก String เป็นตัวเลข

---

## 📌 **13. ตัวอย่างโปรแกรม Java**

### **โปรแกรม HelloWorld**
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

### **โปรแกรมคำนวณดอกเบี้ย (Interest.java)**
```java
public class Interest {
    public static void main(String[] args) {
        double principal = 17000;
        double rate = 0.07;
        double interest = principal * rate;
        principal = principal + interest;

        System.out.println("The interest earned is $" + interest);
        System.out.println("The value after one year is $" + principal);
    }
}
```

---

## 📌 **14. ตัวอย่างการใช้ Enum**
```java
public class EnumDemo {
    enum Day { SUNDAY, MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY }
    public static void main(String[] args) {
        Day tgif = Day.FRIDAY;
        System.out.println(tgif + " is the " + tgif.ordinal() + "-th day of the week.");
    }
}
```

---

## ✅ **เคล็ดลับสำคัญสำหรับการสอบ**
1. เข้าใจกฎการเขียนโค้ด Java (Syntax Rules)
2. จำชนิดข้อมูลพื้นฐานและการประกาศตัวแปรให้ได้
3. เข้าใจแนวคิด **Black-Box** และการใช้ Subroutine
4. ฝึกเขียนโปรแกรมที่ใช้ Math และ String
5. รู้จักการใช้ Enum และการรับค่า Arguments ในโปรแกรม

---

ถ้าต้องการให้ช่วยสร้างคำถามสำหรับฝึกสอบ หรืออยากได้สรุปเพิ่มเติมในส่วนไหน แจ้งมาได้เลยครับ 😊
