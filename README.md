# JAVA
Java is a programming language and computing platfrom which is fast, secure, and reliable. Java is used everywhere from laptops to datacenters, game consoles to scientific supercomputers, cell phones to the Internet. 

### Java Variables
A variable is a container which holds the value while the Java Program is executed. A variable is assigned with a data type. There are three types of variables in java:
 * local
 * instance
 * Static

 #### Local Variable
 A variable declared inside the body of the method is called local variable. You can use this variable only within that method and the other methods in the class aren't even aware that the variable exists.

A local variable cannot be defined with "static" keyword.

#### Instance Variable
A variable declared inside the class but outside the body of the method, is called instance variable. It is not declared as static.

It is called instance variable because its value is instance specific and is not shared among instances.

#### Static Varible
A variable which is declared as static is called static variable. It cannot be local. You can create a single copy of static variable and share among all the instances of the class. Memory allocation for static variable happens only once when the class is loaded in the memory.

#### Example to understand the types of Variables
```java
class A{  
int data=5;//instance variable  
static int m=10;//static variable  
void method(){  
int n=9;//local variable  
}  
}//end of class
```
### Data Types in Java
 Data types specify the different sizes and values that can be stored in the variable. There are two types of data types in Java:

* Primitive data types: The primitive data types include boolean, char, byte, short, int, long, float and double.
* Non-primitive data types: The non-primitive data types include Classes, Interfaces, and Arrays.

#### Java Primitive Data Types
In Java language, primitive data types are the building blocks of data manipulation. These are the most basic data types available in Java language.
There are 8 types of primitive data types:
* boolean data type
* byte data type
* char data type
* short data type
* int data type
* long data type
* float data type
* double data type

![Java Data Types](https://github.com/devrajadhikari333/JAVA_info/blob/master/images/data_types.PNG)

![Java Data Types Size](https://github.com/devrajadhikari333/JAVA_info/blob/master/images/data_types_size.PNG)

##### Boolean Data Type
The boolean data type is used to store only two possible values: true and false. This data type is only used to varify the true or false conditions.
The Boolean data type specifies one bit of information, but its "size" can't be defined precisely.
**Example: Boolean one = false**
 ##### Byte Data Type
 It is an 8-bit signed two's complement integer. Its minimum value is -128 and maximum value is 127. Its default value is 0.
 The byte data type is used to save memory in large arrays where the memory savings is most required. It saves space because a byte is 4 times smaller than an integer. It can also be used in place of "int" data type.
 **Example: byte a = 10, byte b = -20**
 ##### Short Data Type
 The short data type is a 16-bit signed two's complement integer. Its value-range lies between -32,768 to 32,767 (inclusive). Its minimum value is -32,768 and maximum value is 32,767. Its default value is 0.
 The short data type can also be used to save memory just like byte data type. A short data type is 2 times smaller than an integer.
 **Example: short s = 10000, short r = -5000**
 ##### Int Data Type
 The int data type is a 32-bit signed two's complement integer. Its value-range lies between - 2,147,483,648 (-2^31) to 2,147,483,647 (2^31 -1) (inclusive). Its minimum value is - 2,147,483,648and maximum value is 2,147,483,647. Its default value is 0.
The int data type is generally used as a default data type for integral values unless if there is no problem about memory.
**Example: int a = 100000, int b = -200000**
 ##### Long Data Type
 The long data type is a 64-bit two's complement integer. Its value-range lies between -9,223,372,036,854,775,808(-2^63) to 9,223,372,036,854,775,807(2^63 -1)(inclusive). Its minimum value is - 9,223,372,036,854,775,808and maximum value is 9,223,372,036,854,775,807. Its default value is 0. The long data type is used when you need a range of values more than those provided by int.
**Example: long a = 100000L, long b = -200000L**
##### Float Data Type
The float data type is a single-precision 32-bit IEEE 754 floating point.Its value range is unlimited. It is recommended to use a float (instead of double) if you need to save memory in large arrays of floating point numbers. The float data type should never be used for precise values, such as currency. Its default value is 0.0F.
**Example: float f1 = 234.5f**
##### Double Data Type
The double data type is a double-precision 64-bit IEEE 754 floating point. Its value range is unlimited. The double data type is generally used for decimal values just like float. The double data type also should never be used for precise values, such as currency. Its default value is 0.0d.
**Example: double d1 = 12.3**
##### Char Data Type
The char data type is a single 16-bit Unicode character. Its value-range lies between '\u0000' (or 0) to '\uffff' (or 65,535 inclusive).The char data type is used to store characters.
**Example: char letterA = 'A'**

### Operators in Java
Operator in Java is a symbol which is used to perform operations. For example: +, -, *, / etc.

There are many types of operators in Java which are given below:
* Unary Operator
* Arithmetic Operator
* Shift Operator
* Relational Operator
* Bitwise Operator
* Logical Operator
* Ternary Operator and
* Assignment Operator

### Java Operator Precedence
![Java Data Types]()

#### Java Unary Operator
The Java unary operators require only one operand. Unary operators are used to perform various operations i.e.:
* incrementing/decrementing a value by one
* negating an expression
* inverting the value of a boolean

**Java Unary Operator Example: ++ and --**
```java
class OperatorExample{  
public static void main(String args[]){  
int x=10;  
System.out.println(x++);//10 (11)  
System.out.println(++x);//12  
System.out.println(x--);//12 (11)  
System.out.println(--x);//10  
}}
```
**Output**
```
10
12
12
10
```
**Java Unary Operator Example 2: ++ and --**
```java
 class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=10;  
System.out.println(a++ + ++a);//10+12=22  
System.out.println(b++ + b++);//10+11=21
}}
```
**Output**
```
22
21
```
**Java Unary Operator Example: ~ and !**
```java
class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=-10;  
boolean c=true;  
boolean d=false;  
System.out.println(~a);//-11 (minus of total positive value which starts from 0)  
System.out.println(~b);//9 (positive of total minus, positive starts from 0)  
System.out.println(!c);//false (opposite of boolean value)  
System.out.println(!d);//true  
}}
```
**Output**
```
-11
9
false
true
```
#### Java Arithmetic Operators
Java arithmatic operators are used to perform addition, subtraction, multiplication, and division. They act as basic mathematical operations.
**Java Arithmetic Operator Example**
```java
class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=5;  
System.out.println(a+b);//15  
System.out.println(a-b);//5  
System.out.println(a*b);//50  
System.out.println(a/b);//2  
System.out.println(a%b);//0  
}}
```
**Output**
```
15
5
50
2
0
```
**Java Arithmetic Operator Example: Expression**
```java
class OperatorExample{  
public static void main(String args[]){  
System.out.println(10*10/5+3-1*4/2);  
}}
```
**Output**
```
21
```
#### Java Left Shift Operator
The Java left shift operator << is used to shift all of the bits in a value to the left side of a specified number of times.
**Java Left Shift Operator Example**
```java
class OperatorExample{  
public static void main(String args[]){  
System.out.println(10<<2);//10*2^2=10*4=40  
System.out.println(10<<3);//10*2^3=10*8=80  
System.out.println(20<<2);//20*2^2=20*4=80  
System.out.println(15<<4);//15*2^4=15*16=240  
}}
```
**Output**
```
40
80
80
240
```
#### Java Right Shift Operator
The Java right shift operator >> is used to move left operands value to right by the number of bits specified by the right operand.
**Java Right Shift Operator Example**
```java
class OperatorExample{  
public static void main(String args[]){  
System.out.println(10>>2);//10/2^2=10/4=2  
System.out.println(20>>2);//20/2^2=20/4=5  
System.out.println(20>>3);//20/2^3=20/8=2  
}}  
```
**Output**
```
2
5
2
```
**Java Shift Operator Example: >> vs >>>**
```java
class OperatorExample{  
public static void main(String args[]){  
    //For positive number, >> and >>> works same  
    System.out.println(20>>2);  
    System.out.println(20>>>2);  
    //For negative number, >>> changes parity bit (MSB) to 0  
    System.out.println(-20>>2);  
    System.out.println(-20>>>2);  
}}
```
**Output**
```
5
5
-5
1073741819
```
**Java AND Operator Example: Logical && and Bitwise &**
The logical && operator doesn't check second condition if first condition is false. It checks second condition only if first one is true.

The bitwise & operator always checks both conditions whether first condition is true or false.
```java
class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=5;  
int c=20;  
System.out.println(a<b&&a<c);//false && true = false  
System.out.println(a<b&a<c);//false & true = false  
}}  
```
**Output**
```
false
false
```
**Java AND Operator Example: Logical && vs Bitwise &**
```java
class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=5;  
int c=20;  
System.out.println(a<b&&a++<c);//false && true = false  
System.out.println(a);//10 because second condition is not checked  
System.out.println(a<b&a++<c);//false && true = false  
System.out.println(a);//11 because second condition is checked  
}}  
```
**Output**
```
false
10
false
11
```
**Java OR Operator Example: Logical || and Bitwise |**
The logical || operator doesn't check second condition if first condition is true. It checks second condition only if first one is false.

The bitwise | operator always checks both conditions whether first condition is true or false.
```java
class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=5;  
int c=20;  
System.out.println(a>b||a<c);//true || true = true  
System.out.println(a>b|a<c);//true | true = true  
//|| vs |  
System.out.println(a>b||a++<c);//true || true = true  
System.out.println(a);//10 because second condition is not checked  
System.out.println(a>b|a++<c);//true | true = true  
System.out.println(a);//11 because second condition is checked  
}}  
```
**Output**
```
true
true
true
10
true
11
```
#### Java Ternary Operator
Java Ternary operator is used as one liner replacement for if-then-else statement and used a lot in Java programming. it is the only conditional operator which takes three operands.
**Java Ternary Operator Example**
```java
class OperatorExample{  
public static void main(String args[]){  
int a=2;  
int b=5;  
int min=(a<b)?a:b;  
System.out.println(min);  
}}  
```
**Output**
```
2
```
**Another Example:**
```java
class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=5;  
int min=(a<b)?a:b;  
System.out.println(min);  
}} 
```
**Output**
```
5
```
#### Java Assignment Operator
Java assignment operator is one of the most common operator. It is used to assign the value on its right to the operand on its left.
**Java Assignment Operator Example**
```java
class OperatorExample{  
public static void main(String args[]){  
int a=10;  
int b=20;  
a+=4;//a=a+4 (a=10+4)  
b-=4;//b=b-4 (b=20-4)  
System.out.println(a);  
System.out.println(b);  
}}  
```
**Output**
```
14
16
```