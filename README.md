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

