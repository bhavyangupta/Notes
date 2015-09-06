# Interfaces
- Reference type
- collection of *abstract* methods implemented by a class
- may contain constants, static methods, default methods
- Unless the class implementing an interface is abstract,
  it must **implement all the methods** declared in the interface
  it implements
- An interface cannot contain instance fields -> all fields 
  in an interface **must be static and final**
- An interface can extend multiple interfaces.

## Implementing an interface
- When a class *implements* an interface, it signs a contract 
  to define the methods declared in the interface - otherwise
  the class itself must be declared *abstract*.
- Java interfaces **cannot define methods** .
- A class can implement many interfaces - separate them by commas.

## Extending interfaces
- An interface can extend other interfaces using the *extend* keyword.
- Multiple interfaces can be extended by a given interface.
- When an interface extends one or more interfaces, it inherits all 
  method declarations of the extended interfaces and consequently any
  class implementing this new interface **must** define the methods in 
  all the interfaces combined.

## Thoughts
- Interfaces seem like a cool way to define an API for entities.
- They would also ensure consistency in terms of what behaviour is defined
  for a given entity. For eg, if I declare an interface with some behaviour, 
  I can be assured that all mandatory behaviours I want from an entity **will**
  be defined. 
- This also makes the code more **decoupled** and **stable**.

# Reference:
http://www.tutorialspoint.com/java/java_interfaces.html
http://tutorials.jenkov.com/java/interfaces.html