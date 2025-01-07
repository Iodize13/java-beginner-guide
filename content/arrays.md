### 📚 **สรุปเนื้อหาเรื่อง Arrays (ภาษาไทย พร้อมตัวอย่างโค้ด)**

---

## ✅ **การสร้างและใช้งาน Array**
```java
// สร้าง Array เก็บจำนวนเต็ม 5 ค่า
int[] numbers = new int[5];

// กำหนดค่าใน Array
numbers[0] = 10;
numbers[1] = 20;
numbers[2] = 30;
numbers[3] = 40;
numbers[4] = 50;

// แสดงผลลัพธ์
for (int i = 0; i < numbers.length; i++) {
    System.out.println("Element " + i + ": " + numbers[i]);
}
```

---

## ✅ **Array Initialization (การกำหนดค่าเริ่มต้น)**
```java
// สร้างและกำหนดค่าเริ่มต้นใน Array
int[] list = {1, 2, 3, 4, 5};

// แสดงผลลัพธ์
for (int num : list) {
    System.out.println(num);
}
```

---

## ✅ **Multi-dimensional Arrays (Array หลายมิติ)**
```java
// สร้าง 2D Array (3 แถว 4 คอลัมน์)
int[][] matrix = {
    {1, 2, 3, 4},
    {5, 6, 7, 8},
    {9, 10, 11, 12}
};

// แสดงผลลัพธ์
for (int i = 0; i < matrix.length; i++) {
    for (int j = 0; j < matrix[i].length; j++) {
        System.out.print(matrix[i][j] + " ");
    }
    System.out.println();
}
```

---

## ✅ **การค้นหาค่าใน Array (Linear Search)**
```java
public class LinearSearch {
    public static int search(int[] array, int target) {
        for (int i = 0; i < array.length; i++) {
            if (array[i] == target) {
                return i;  // คืนค่า index ที่เจอ
            }
        }
        return -1;  // คืนค่า -1 ถ้าไม่เจอ
    }

    public static void main(String[] args) {
        int[] numbers = {10, 20, 30, 40, 50};
        int index = search(numbers, 30);
        System.out.println("Found at index: " + index);  // ผลลัพธ์: Found at index: 2
    }
}
```

---

## ✅ **การคัดลอกค่าใน Array (Array Copy)**
### 📋 **วิธีที่ 1: การคัดลอกแบบ Manual**
```java
int[] source = {1, 2, 3, 4, 5};
int[] destination = new int[source.length];

// คัดลอกค่า
for (int i = 0; i < source.length; i++) {
    destination[i] = source[i];
}

// แสดงผลลัพธ์
for (int num : destination) {
    System.out.println(num);
}
```

### 📋 **วิธีที่ 2: การคัดลอกด้วย System.arraycopy()**
```java
int[] source = {1, 2, 3, 4, 5};
int[] destination = new int[source.length];

// ใช้ System.arraycopy() ในการคัดลอก
System.arraycopy(source, 0, destination, 0, source.length);

// แสดงผลลัพธ์
for (int num : destination) {
    System.out.println(num);
}
```

---

## ✅ **การเรียงลำดับค่าใน Array (Sorting)**
### 📋 **การเรียงลำดับด้วย Insertion Sort**
```java
public class InsertionSort {
    public static void sort(int[] array) {
        for (int i = 1; i < array.length; i++) {
            int key = array[i];
            int j = i - 1;

            while (j >= 0 && array[j] > key) {
                array[j + 1] = array[j];
                j--;
            }
            array[j + 1] = key;
        }
    }

    public static void main(String[] args) {
        int[] numbers = {5, 2, 9, 1, 5, 6};
        sort(numbers);

        for (int num : numbers) {
            System.out.print(num + " ");  // ผลลัพธ์: 1 2 5 5 6 9
        }
    }
}
```

---

## ✅ **การค้นหาด้วย Binary Search (Binary Search)**
```java
public class BinarySearch {
    public static int binarySearch(int[] array, int target) {
        int low = 0;
        int high = array.length - 1;

        while (low <= high) {
            int mid = (low + high) / 2;

            if (array[mid] == target) {
                return mid;  // คืนค่า index ที่เจอ
            } else if (array[mid] < target) {
                low = mid + 1;
            } else {
                high = mid - 1;
            }
        }
        return -1;  // คืนค่า -1 ถ้าไม่เจอ
    }

    public static void main(String[] args) {
        int[] numbers = {1, 2, 3, 4, 5, 6, 7, 8, 9};
        int index = binarySearch(numbers, 5);
        System.out.println("Found at index: " + index);  // ผลลัพธ์: Found at index: 4
    }
}
```

---

## ✅ **การใช้ Arrays Utility ใน Java**
```java
import java.util.Arrays;

public class ArrayUtilityExample {
    public static void main(String[] args) {
        int[] numbers = {5, 2, 9, 1, 5, 6};

        // เรียงลำดับ Array
        Arrays.sort(numbers);

        // แสดงผลลัพธ์หลังเรียงลำดับ
        System.out.println(Arrays.toString(numbers));  // ผลลัพธ์: [1, 2, 5, 5, 6, 9]

        // ค้นหาด้วย Binary Search
        int index = Arrays.binarySearch(numbers, 5);
        System.out.println("Found at index: " + index);  // ผลลัพธ์: 2
    }
}
```

---

ต้องการให้สรุปหัวข้ออื่นต่อไหมครับ เช่น **Recursion**, **Multi-dimensional Arrays** หรือหัวข้ออื่นที่ต้องการเน้นเป็นพิเศษ? 😊

