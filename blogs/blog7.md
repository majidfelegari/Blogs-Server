# Understanding Data Types in Kotlin  

## Introduction  

Kotlin is a **statically typed** language, meaning every variable and value has a specific data type that is known at **compile time**. Data types define what kind of values a variable can store and what operations can be performed on it.  

In Kotlin, data types are divided into different categories:  

- **Numbers (Int, Long, Float, Double, Byte, Short)**  
- **Characters (Char)**  
- **Boolean (true/false values)**  
- **Strings (Text values)**  
- **Arrays (Collection of elements)**  

---

## **1. Number Types in Kotlin**  

Kotlin supports different types of numbers depending on their size and precision:  

| Data Type  | Size (Bits) | Range |
|------------|------------|--------------------------|
| `Byte`     | 8          | -128 to 127 |
| `Short`    | 16         | -32,768 to 32,767 |
| `Int`      | 32         | -2,147,483,648 to 2,147,483,647 |
| `Long`     | 64         | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 |
| `Float`    | 32         | 6-7 decimal digits precision |
| `Double`   | 64         | 15-16 decimal digits precision |

### **Example Usage:**  
```kotlin
val age: Int = 25
val distance: Long = 1_000_000L
val pi: Float = 3.14F
val price: Double = 99.99
```

---

## **2. Characters (`Char`)**  

A `Char` represents a **single character** and is enclosed in **single quotes** (`'A'`, `'B'`, `'1'`).  

### **Example Usage:**  
```kotlin
val grade: Char = 'A'
val digit: Char = '9'
```

---

## **3. Boolean (`Boolean`)**  

A `Boolean` type has **only two values**:  
- `true`  
- `false`  

### **Example Usage:**  
```kotlin
val isKotlinFun: Boolean = true
val isUserLoggedIn: Boolean = false
```

---

## **4. Strings (`String`)**  

A `String` is a **sequence of characters**, enclosed in **double quotes** (`"Hello, Kotlin!"`). Strings in Kotlin are immutable (cannot be changed after creation).  

### **Example Usage:**  
```kotlin
val name: String = "John Doe"
val message: String = "Welcome to Kotlin!"
```

#### **String Interpolation (Using Variables in Strings)**
Kotlin allows embedding variables inside strings using **`$`**:
```kotlin
val user = "Alice"
println("Hello, $user!")  // Output: Hello, Alice!
```

---

## **5. Arrays (`Array`)**  

An `Array` is a collection of elements of the **same type**, stored in a fixed-size list.  

### **Example Usage:**  
```kotlin
val numbers = arrayOf(1, 2, 3, 4, 5)
val fruits = arrayOf("Apple", "Banana", "Cherry")
```

You can access elements by **index (starting from 0)**:  
```kotlin
println(numbers[0])  // Output: 1
println(fruits[1])   // Output: Banana
```

---

## **Type Inference in Kotlin**  

Kotlin can **automatically detect** the type of a variable, so you **don’t need to explicitly specify it**:
```kotlin
val age = 25       // Kotlin infers this as Int
val pi = 3.14      // Kotlin infers this as Double
val isAdult = true // Kotlin infers this as Boolean
```
This feature makes Kotlin **more concise and readable**.

---

## **Conclusion**  

Kotlin provides a **rich set of data types** to handle different kinds of values efficiently. Understanding these data types is essential for writing **clean, efficient, and bug-free** Kotlin code.  

By leveraging **type inference**, **immutability**, and **string interpolation**, Kotlin makes working with data types easy and intuitive. 🚀  

Now that you understand Kotlin’s data types, you’re ready to start writing more powerful Kotlin programs!🚀😊  
