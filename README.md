java
====

Contents
--------


## Objects and classes

An __object__ can be considered a "_thing_" that can perform a set of related activities. In OOP terms an object is an instance of a class.

A __class__ is the template that describe the details of an object.

The following is a Java class named _Bicycle_:

<!-- language: java -->

    public class Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

    void changeCadence(int newValue) {
         cadence = newValue;
    }

    void changeGear(int newValue) {
         gear = newValue;
    }

    void speedUp(int increment) {
         speed = speed + increment;   
    }

    void applyBrakes(int decrement) {
         speed = speed - decrement;
    }

    void printStates() {
         System.out.println("cadence:" +
             cadence + " speed:" + 
             speed + " gear:" + gear);
    }
    }

A new object of the _Bicycle_ class can be instantiated using the following statement: 

    Bicycle bike = new Bicycle();
    
## Variables

* There are several kinds of variables:
    - Member variables in a class—these are called __fields__.
    - Variables in a method or block of code—these are called __local variables__.
    - Variables in method declarations—these are called __parameters__.
    - Variables which are defined without the _static_ keyword  and are _outside any method declaration_ are object specific and are known as __instance variables__.

### Local variables

* __Final__ is the _Only Non Access Modifier_ that can be applied to a local variable.
* Local variables are not assigned a default value, hence they __need to be initialized__.

### Instance variables

* Can use any of the four access level
* Can be marked final
* Can be marked abstract
* Can not be marked static

### Reference variables

## Constructors

* Constructor declarations look like method declarations—except that they use the name of the class and have no return type.

## Packages

* The package statement MUST be the first line in the source file.
* There can be only one package statement in each source file.
* Package names are written in all lower case to avoid conflict with the names of classes or interfaces.
* Package names can contain underscores.
* Companies use their reversed Internet domain name to begin their package names—for example, com.example.mypackage for a package named mypackage created by a programmer at example.com.

## Access modifiers

### Access modifiers for class

* Classes in Java can use only __public__ and __default__ access modifiers.
* When set to __public__, the given class will be accessible to all the classes available in Java world.
* When set to __default__, the given class will be accessible to the classes which are defined in the __same package__.

<img src="resources/access_modifiers_class.png" width="350" height="100">

### Access modifiers for variable

* Variables in Java can use the following access modifiers: __default__, __private__, __protected__, __public__.
* If a variable is set to __default__, it will be accessible to the classes which are defined in the same package. 
* If a variable is set to __public__ it can be accessible from any class available in the Java world.
* If a variable is set to __protected__ inside a class, it will be accessible from its sub classes defined in the same or different package only via Inheritance.
* A variable if defined __private__ will be accessible only from within the class it is defined.

<img src="resources/access_modifiers_variables.png" width="500" height="250">

### Access modifiers for method

* Methods in Java can use the following access modifiers: __default__, __private__, __protected__, __public__.
* When a method is set to __default__ it will be accessible to the class which are defined in the same package.
* When a method is set to __public__ it will be accessible from any class available in the Java world.
* If a method is set to __protected__ inside a class, it will be accessible from its sub classes defined in the same or different package.
* A method if defined __private__ will be accessible only from within the class it is defined. 

<img src="resources/access_modifiers_methods.png" width="500" height="250">

## Non-access modifiers

### Static keyword

* Applicable to:
    - method
    - variable
    - class nested within another class
    - initialization block
* Not applicable to:
    - class (not nested)
    - constructor
    - interfaces
    - inner class methods
    - instance variables
    - local variables
* Variables/methods having the __static__ keyword are common to all objects. 
* Fields that have the static modifier in their declaration are called __static fields__ or __class variables__. They are associated with the class, rather than with any object. 
* Any object can change the value of a class variable, but class variables can also be manipulated without creating an instance of the class.

### Final

Final modifiers are applicable to:
* Class : A class when set to final __cannot be extended__ by any other class
* Method : A method when set to final __cannot be overridden__ by any subclass
* Variable : When a variable is set to final, its value __cannot be changed__. Final variables are like constants.


### Abstract

Abstract modifiers are applicable to:
* Class
* Method

#### Abstract class

* An abstract class can have abstract methods.
* A class can also be an abstract class without having any abstract methods in it. 
* If a class has an abstract method, the class becomes an abstract class.

#### Abstract methods

* Abstract methods do not have an implementation.
* Abstract methods have only a signature (they don't have body).

## Interfaces
* Interfaces can be defined with __interface__ keyword.

<!-- language: java -->
    public interface MyInterface
    {
    int i=0;
    public void Height(int height);
    public abstract void setHeight();
    }
    
* All Interface methods are implicitly __public__ and __abstract__.
* Interfaces can declare only __constants__. Instance variables are not allowed. It means all variables inside an Interface must be __public, static, final__. Variables inside interface are implicitly public static final.
* Interface methods can not be static.
* Interface can _extend_ one or more other interface.

## Polimorphysm

## String class

* The String class represents character strings. All string literals in Java programs, such as “abc”, are implemented as instances of this class.
* String objects are immutable.
* How to create:

<!-- language: java -->

    String str = new String(“abc”);
    String str1 = "abc";

* Important methods of the String class:
    - length()
    - charAt(int index)
    - concat(String str)
    - contains(CharSequence s)
    - equals(Object anObject)
    

## References

* [http://docs.oracle.com/javase/tutorial/java/](http://docs.oracle.com/javase/tutorial/java/)
* [http://javabeginnerstutorial.com/core-java/](http://javabeginnerstutorial.com/core-java/)
