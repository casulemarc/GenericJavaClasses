## Generic Classes In Java
Project to test for the use of generic classes in Java.

## What is a generic class?
A generic class is a class that can operate on a specific type specified by the programmer at compile time. These classes take a type as a parameter. They are particularly useful for collection classes e.g ArrayLists, HashMap, HashSet.
A generic can extend generic and non-generic classes.
In the notation <T extends Number>, the Number class specifies an upper bound for the parameter type T.

## What is legal syntax for using a generic class?
We use <> to specify a Parameter type. We don’t use int, double.

### CLASS:
public class GentType <T> {
	/*Statements*/
} 
### INSTANCE OF GENERIC CLASS
GenType < Integer> something = new GenType<Integer>(/*data value to be passed*/);
If two parameters are to taken <T, U>, then pass two values as well.

### PARAMETERIZED TYPES
OrderedPair<String, Box<Integer>> p = new OrderedPair<>("primes", new Box<Integer>(...));

### What happens when a client calls a generic method?
The compiler determines the actual types to use for the type parameters from the context.

### What are the benefits of using a generics class?
•	More type problems can be uncovered at compile-time rather than at run time.
•	Increased type-safety without the need to do typecasts at run time.
•	Generics promotes code reusability.
•	Individual Type Casting is not needed

### When you create an instance of a generic class, what types can you pass as arguments for the class type parameters?
Refence types only can be passed.

### The automatic conversion of a primitive type to the corresponding wrapper type when being passed as parameter to a generic class is called AutoBoxing
### When a generic class with an unconstrained type parameter is instantiated without specifying an actual type argument: 
The Object type is replaced to be used as the unspecified type.
GenType <> something = new GenType<>(/*data value to be passed*/);

### When a generic class is instantiated without specifying an actual type argument, the generic class is being used as a raw type.

### In a generic method, a type parameter is defined before the method’s return type.
### Comparable<T> is an interface defined in the Java class libraries to compare items like in an array.
### Erasure is the process of replacing generic types with their upper bound, or with Object, during compilation.
### Which of the following statements is true? Generic types do not exist at the byte code level.
### Exceptions of a generic type are not permitted in Java

### Output

<img width="525" alt="ResultOutput" src="https://user-images.githubusercontent.com/75389946/133317719-3a253291-0a18-487d-8444-eeb0ed102df4.png">

