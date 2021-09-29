# notes
## Week of Sept 27

**UML Diagram
* + public
* - private
* # Protected
* ~ Package
**CLasses as Contracts
* Superclass makes certain promises about available methods and instance variables
* Child classes keep these promises
* Implementation of these promises can be overwritten

* Sometimes a superclass needs to make a promise, but can't provide implementation.
* Example:

```java
public abstract class Product{
  protected double price;
  
}
```
* abstract cannot be instantiated, but can be used as types
* Produce p = new Apple();
* no: Produe p = new Produce();
* Enables the writing of methods that can interface with abstract methods
* The produce can call the methods implemented within Apple

```java
ArrayList<Produce> L =
  new ArrayList<Produce>();
 L.add(new Apple(0.5, 3.5));
 L.add(new Orange(2.5, 4.25));
```
Essentially, produce is a type of object. The type allows you to access the objects of type produce.

**Properties of Abstract Classes
* These constructors are protected or private
* Child classes can reference these with super()
* Could be the default constructor

* Provide as many method implementations as possible
* These implementations may call abstract methods
  * The methods will ultimately be implemented by the child classes (or grandchildren.
  * IT is these concrete classes that ensure all methods are implemented.

**ArrayList
All implemented interfaces
* Serializable
* Cloneable
* Iterable
* Collection
* List
* RandomAccess
  
**Java Restriction
* An interface defines to implementation - only a set of abstract methods.
* All checks can be mate at compile time, so the runtime cost is low.
* It is a class-like construct


We can extend a different class and still make the same guarantees as those provided by cloneable:
```java
public class Apple extends Fruit implements Cloneable{

}
```
A class can implement any number of interfaces.
  




## Week of Sept 10 2021
* Testing bullet points
* Another Bullet
* Yet another
* AND ANOTHER ONE

###How to add code within text

```java
final int BIG = 1000000000;
```

During this class we learned about using jshell for a few things. We tried using different infinities and realized a computer doesn't know infinity. 

```java
Integer.MAX_VALUE
DOUBLE.MAX_VALUE + 1
```

**NOTE**

Use _JSHELL_ to experiment
