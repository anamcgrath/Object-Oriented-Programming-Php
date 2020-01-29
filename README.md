# Object-Oriented-Programming-Php
Object Oriented Programming uses objects and classes to minimize the amount of code needed to build web applications.

## What is Object Oriented Programming?
Object Oriented Programming (OOP) is about making objects that contain both data and functions. OOP is used to build complex and reusable web applications in web development. OOP minimizes the length of code, making it clear and simpler to modify.

## How is Object Oriented Programming used in PHP?
  OOP is made up of classes and objects, classes are the broader term or template that is made up of multiple objects, objects have the same properties that the class said they would have but the property values may be different. Classes are generic but an object has to be specific. There can be many objects for one class.
  
### Example
  
  ```
 <?php
 
  class colour {
    public primarycolour($pChoose) {
      echo "This is a primary colour: " . $pChoose;
     }
    public secondarycolour($sChoose) {
      echo "This is a secondary colour: " . $sChoose;
    }
  }
  class shade extends colour {
     public highlight($hChoose) {
       echo "This is a highlight: " . $hChoose;
      }
     public shadow($shChoose) {
       echo "This is a shadow: " . $shChoose;
      }
  }
?>
```

The above example 
