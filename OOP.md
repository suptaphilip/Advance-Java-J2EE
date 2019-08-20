# City University
#### Object oriented programming
##### Lecture 3
Supta Richard Philip
supta.philip@gmail.com
****


The main goal of OOP is to bind data and code(methods) togather.

> ## OOP provide few concepts
> 
> ### 1.  Encapsulation

* Encapsulation in Java is a process of wrapping code and data together into a single unit.
* create a fully encapsulated class in Java by making private all the data members of the class. 
*  use setter and getter methods to set and get the data in it.
* The Java Bean class or POJO class is the example of a fully encapsulated class.
* Class Diagram of Student

![student class diagram](https://github.com/suptaphilip/Advance-Java-J2EE/raw/J2EE/Student-Class1.png)

Student.java
```java
package org.cityU.Encapsulation;

public class Student {
	
	private String name;

	public String getName() {
		return name;
	}

	public void setName(String name) {
		this.name = name;
	}
}

``` 
StudentTest.java

```java
package org.cityU.Encapsulation;

public class StudentTest {

	public static void main(String[] args) {

		Student s = new Student();
		s.setName("Richard");
		
		System.out.println(s.getName());
	}
}

```
> ### 2.   Abstraction
* Abstraction is a process of hiding the implementation details and showing only functionality to the user.
* There are two ways to achieve abstraction in java
	- Abstract class (0 to 100%)
	- Interface (100%)
	
![Abstaction class diagram](https://github.com/suptaphilip/Advance-Java-J2EE/raw/J2EE/Abstract2.png)	
	
```java
abstract class Bank {
	abstract int getRateOfInterest();
}

class SBI extends Bank {
	int getRateOfInterest() {
		return 7;
	}
}

class PNB extends Bank {
	int getRateOfInterest() {
		return 8;
	}
}

class TestBank {
	public static void main(String args[]) {
		Bank b;
		b = new SBI();
		System.out.println("Rate of Interest is: " + b.getRateOfInterest() + " %");
		b = new PNB();
		System.out.println("Rate of Interest is: " + b.getRateOfInterest() + " %");
	}
}
```
Same examples you can solve with interface.

![Abstaction using Interface](https://github.com/suptaphilip/Advance-Java-J2EE/raw/J2EE/Interface.png)	

> ### 3.   Polymorphism
* Polymorphism in Java is a concept by which we can perform a single action in different ways.
* There are two types of polymorphism in Java: compile-time polymorphism and runtime polymorphism.

#### Runtime polymorphism using interface and method overriding 

![Runtime Polymorphism using Interface](https://github.com/suptaphilip/Advance-Java-J2EE/raw/J2EE/RuntimePolymorphism.png)

#### Compiletime polymorphism using method overloading
![Compiletime Polymorphism using method overloading ](https://github.com/suptaphilip/Advance-Java-J2EE/raw/J2EE/CompileTimePolymorphism.png)
> ### 4.   Inheritance
* Inheritance in Java is a mechanism in which one object acquires all the properties and behaviors of a parent object.
* create new classes that are built upon existing classes.
* Inheritance represents the IS-A relationship which is also known as a parent-child relationship.

```java

```

> Watch the video tutorials

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/4AjCAKZPCOM/1.jpg)](https://www.youtube.com/watch?v=4AjCAKZPCOM&list=PLzS3AYzXBoj88SIyxN_6LWh92S-_49tlJ)

> Apart from these, there are some other concepts which are used in Object-Oriented design:

* Coupling
* Cohesion
* Association
* Aggregation
* Composition
