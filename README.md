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

A new object of the _Bicycle_ class can be instantiated using the following line: 

    Bicycle bike = new Bicycle();
    
## Access modifiers

## Non-access modifiers

## Interfaces

## Polimorphysm

## Variables

## Constructors

## Package


