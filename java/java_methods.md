# Methods
##  Method Overriding 
* You cannot change the method name, type, parameters
  when you override a function. In **Overloading**,
  on the other hand, you are free do what ever you want.

## Passing Command Line Arguments
* Arguments are passed to main 
* Main is passed an array of string[] arguments when you run
  the program. Each element of the array is an argument. 
  Arguments are differentiated by spaces in the command.

## Constructors
* Java provides default constructors - that initialises
  everything to zero. 

##  *this* keyword
* Used as a reference to the object of the current class.
* Used to differentiate instance variables and local vars and
  avoid name conflicts.
* *Explicit constructor invocation* - used to invoke a different
  kind of contructor from a given constructor of the same class.

```java
class Student{

 int age
 Student(){
 this(20);
 }
 
 Student(int age){
 this.age=age;  
 }

}
```


## Variable Arguments (var-args)
* Available in Java 5 onwards
* Allows you to pass variable number of arguments of the same
  type to a method.
* Only **one** variable length parameter may be specified in a method
  and it has to be the **last** parameter.
* Example:
  ```java
  public class VarargsDemo {

     public static void main(String args[]) {
        // Call method with variable args  
      printMax(34, 3, 3, 2, 56.5);
        printMax(new double[]{1, 2, 3});
     }

     public static void printMax( double... numbers) {
     if (numbers.length == 0) {
        System.out.println("No argument passed");
        return;
     }

     double result = numbers[0];

     for (int i = 1; i <  numbers.length; i++)
        if (numbers[i] >  result)
        result = numbers[i];
        System.out.println("The max value is " + result);
     }
  }

  ```

## *finalize* method
* Automaticallyh called before the object's final destruction by garbage collector.
* Can be used to perform clean-up tasks like closing files.
  ```java
  protected void finalize( )
  {
     // finalization code here
  }
  ```

# Reference
http://www.tutorialspoint.com/java/java_methods.htm