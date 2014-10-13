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
    
## Access modifiers

## Non-access modifiers

### Static keyword

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

## Variables

### Local variables

### Instance variables

### Reference variables

## Constructors

## Packages

## String class


