# CLASS , What is it ?
ECMAScript 2015, also known as ES6, introduced JavaScript Classes.
ECMAScript 2015, also known as ES6, introduced JavaScript Classes.
Always add a method named constructor():
Use the keyword class to create a class.
// Synatx
class Name{
    constructor()
    {}
}

# class
A class is a blueprint for the object. You can create 
an object from the class.
You can think of the class as a sketch (prototype) of 
a house. It contains all the details about the floors, 
doors, windows, etc. Based on these descriptions, 
you build the house. House is the object.
Since many houses can be made from the same 
description, we can create many objects from a class

# Creating JavaScript Class
JavaScript class is similar to the Javascript constructor function, and it 
is merely a syntactic sugar. The constructor function is defined as:

function Odamcha (){
    this.name="Eraj"
    this.age=10
}
const person=new Odamcha()
console.log(person)

Instead of using the function keyword, you use the class keyword for
creating JS classes. For example,

class Person {
    constructor(name){
this.name=name;
    }
}

The class keyword is used to create a class. The properties are assigned
in a constructor function.
Now you can create an object. For example

class Person {
    constructor(name){
this.name=name;
    }
}
let person= new Person("Burut");
let person1= new Person("Aslidin");

Here, person1 and person2 are objects of Person class.

# Note: The constructor() method inside a class gets called
# automatically each time an object is created

# Javascript Class Methods : Getters and Setters
In JavaScript
getter methods get the value of an object 
setter methods set the value of an object.
JavaScript classes may include getters and setters You use
the get keyword for getter methods and set for setter methods. For
example

# example

class Person {
    constructor(name){
this.name=name;
    }
    get personName(){
        return this.name;
    }
    set personName(x){
        this.name=x;
    }
}
let person= new Person("Burut");
person.personName="Sarah"
console.log(person.personName)

# Hoisting
A class should be defined before using it. Unlike functions and other 
JavaScript declarations, the class is not hoisted. For example,

// Eror
let person= new Person("Burut");
console.log(person.personName)
class Person {
    constructor(name){
this.name=name;
    }
}

# use strict
Classes always follow 'use-strict'. All the code inside the class is
automatically in strict mode. For example,
class Person{
    constructor(){
       let  a=0;
        this.name=a
    }
}
let p= new Person()
console.log(p)

Note: JavaScript class is a special type of function. And
the typeof operator returns function for a class. 