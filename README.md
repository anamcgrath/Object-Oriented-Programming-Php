# Object-Oriented-Programming-Php
Object Oriented Programming uses objects and classes to minimize the amount of code needed to build web applications.

## What is Object Oriented Programming?
Object Oriented Programming (OOP) is about making objects that contain both data and functions. OOP is used to build complex and reusable web applications in web development. OOP minimizes the length of code, making it clear and simpler to modify.

## How is Object Oriented Programming used in PHP?
  OOP is made up of classes and objects, classes are the broader term or template that is made up of multiple objects, objects have the same properties that the class said they would have but the property values may be different. Classes are generic but an object has to be specific. There can be many objects for one class.
  
### Example
 #### Input: 
  ```
 <?php
 
  class colour {
    public primarycolour($pChoose) {
      echo "This is a primary colour: " . $pChoose . "<br>";
     }
    public secondarycolour($sChoose) {
      echo "This is a secondary colour: " . $sChoose . "<br>";
    }
  }
  class shade extends colour {
     public highlight($hChoose) {
       echo "This is a highlight: " . $hChoose . "<br>";
      }
     public shadow($shChoose) {
       echo "This is a shadow: " . $shChoose . "<br>";
      }
  }
  $colour = new colour();
  $shade = new shade();
  $colour->primarycolour("red");
  $colour->secondarycolour("green");
  $shade->highlight("bright");
  $shade->shadow("dark");

?>
```
#### Output: 
```
This is a primary colour: red
This is a secondary colour: green
This is a highlight: bright
This is a shadow: dark
```
The above is an example of Object Oriented Programming. The keyword new initiates the function to run. You can access the method of the class by using the object followed by the `->` operator. 


### Example (Using the "this" method)
```
<?php

class fruit {
  public $name;
  public $family;
  
  
  public function fruitName($name, $family){
    $this->name = $name;
    $this->family = $family;
  }
  
  public function text() {
    echo "My favourite fruit is {$this->name} and the family it comes from is {$this->family}";
  }
}

class apple extends fruit {
  public function text() {
      echo "I like apples";
  }
}

?>
```
The above example uses the "This" keyword. It refers to the current object and can only be changed inside of the methods. 
