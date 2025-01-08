### 📚 **Important Details with Slide References (ภาษาไทย พร้อมโค้ดและเลขสไลด์)**

---

### ✅ **1. Array Index Out of Bounds Exception**  
📌 **Slide: Arrays (Slide 11)**  
หากพยายามเข้าถึง index ที่ไม่มีใน array จะเกิดข้อผิดพลาด `ArrayIndexOutOfBoundsException`  
```java
int[] list = {1, 2, 3};
System.out.println(list[3]);  // จะเกิด ArrayIndexOutOfBoundsException
```

---

### ✅ **2. Property `length` ใน Array หลายมิติ**  
📌 **Slide: Arrays (Slide 55)**  
- `A.length` ให้จำนวนแถวของ array  
- `A[0].length` ให้จำนวนคอลัมน์ในแถวแรก  
```java
int[][] A = {
    {1, 2, 3, 4},
    {5, 6, 7, 8},
    {9, 10, 11, 12}
};

System.out.println("Number of rows: " + A.length);        // ผลลัพธ์: 3
System.out.println("Number of columns in row 0: " + A[0].length);  // ผลลัพธ์: 4
```

---

### ✅ **3. Short-Circuit Boolean Operators (`&&` และ `||`)**  
📌 **Slide: Operations, Packages, and Programming Styles (Slide 14)**  
ตัวดำเนินการแบบ `&&` และ `||` ใช้การประเมินค่าแบบ **short-circuit**  
```java
int x = 0;
if (x != 0 && (10 / x) > 1) {
    System.out.println("This will not be printed.");
}
```

---

### ✅ **4. Recursive Method Stopping Condition**  
📌 **Slide: Methods (Slide 27)**  
ถ้า Recursive Method ไม่มีเงื่อนไขหยุด จะทำให้เกิด **StackOverflowError**  
```java
static int factorial(int n) {
    if (n == 0) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}
```

---

### ✅ **5. Parameters Passed by Value**  
📌 **Slide: Methods (Slide 16-18)**  
Java ส่งพารามิเตอร์แบบ **pass by value** เสมอ  
```java
public static void swap(int a, int b) {
    int temp = a;
    a = b;
    b = temp;
    System.out.println("Inside swap: a = " + a + ", b = " + b);
}

public static void main(String[] args) {
    int x = 10;
    int y = 20;
    swap(x, y);
    System.out.println("Outside swap: x = " + x + ", y = " + y);
}
```

👉 **ผลลัพธ์**:
```
Inside swap: a = 20, b = 10
Outside swap: x = 10, y = 20
```

---

### ✅ **6. Overloading Methods**  
📌 **Slide: Methods (Slide 23-25)**  
Java อนุญาตให้สร้าง Method ชื่อเดียวกันได้ หากจำนวนพารามิเตอร์หรือชนิดข้อมูลต่างกัน  
```java
public static int add(int a, int b) {
    return a + b;
}

public static double add(double a, double b) {
    return a + b;
}
```

---

### ✅ **7. การคัดลอกค่าใน Array ด้วย `System.arraycopy()`**  
📌 **Slide: Arrays (Slide 28)**  
Java มี method สำหรับคัดลอกค่าใน array  
```java
int[] source = {1, 2, 3, 4, 5};
int[] destination = new int[source.length];
System.arraycopy(source, 0, destination, 0, source.length);

for (int num : destination) {
    System.out.println(num);
}
```

---

### ✅ **8. การเรียงลำดับค่าใน Array ด้วย Selection Sort**  
📌 **Slide: Arrays (Slide 46)**  
Selection Sort เป็นหนึ่งในอัลกอริทึมที่ใช้เรียงลำดับค่าใน Array  
```java
public class SelectionSort {
    public static void sort(int[] array) {
        for (int i = 0; i < array.length - 1; i++) {
            int minIndex = i;
            for (int j = i + 1; j < array.length; j++) {
                if (array[j] < array[minIndex]) {
                    minIndex = j;
                }
            }
            int temp = array[minIndex];
            array[minIndex] = array[i];
            array[i] = temp;
        }
    }

    public static void main(String[] args) {
        int[] numbers = {64, 25, 12, 22, 11};
        sort(numbers);
        for (int num : numbers) {
            System.out.print(num + " ");  // ผลลัพธ์: 11 12 22 25 64
        }
    }
}
```

---

### ✅ **9. Type Casting and Conversion**  
📌 **Slide: Operations, Packages, and Programming Styles (Slide 22)**  
การแปลงจาก `double` ไปเป็น `int` อาจทำให้ข้อมูลสูญหาย  
```java
double value = 9.99;
int intValue = (int) value;
System.out.println(intValue);  // ผลลัพธ์: 9
```

---

### ✅ **10. การใช้ `continue` และ `break` ใน Loop**  
📌 **Slide: Control (Slide 26-27)**  
- `continue` ข้ามการทำงานในรอบปัจจุบัน และไปเริ่มรอบใหม่  
- `break` หยุดการทำงานของ loop ทันที  
```java
for (int i = 1; i <= 5; i++) {
    if (i == 3) {
        continue;
    }
    if (i == 4) {
        break;
    }
    System.out.println(i);
}
```

👉 **ผลลัพธ์**:
```
1
2
```

---

ถ้ามีส่วนไหนที่ต้องการอธิบายเพิ่มเติม แจ้งได้เลยครับ! 😊
