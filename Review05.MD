________________
# Review Ques 5



1. As precisely as you can (two lines each, at most), define the following.  Your definition should mention inputs,outputs and side-effects:
    - functions

???A function is a block of organized, reusable code that is used to perform a single, related action. No side effect.

    - predictes

Predicate is a function that takes one element as input parameter and return either true or false. Also updates bindings. 

2. Assume a purely logic language where any word starting with upper case is an unbound variable.
   In that logical language what are the outputs and side-effects of the following:
    - emp(tim,42) = emp(Name,Age)
    
    Output : TRUE | Side Effect : Name = tim, Age = 42
    
    - emp(Who,42)  =  emp(tom, Age)
    
    Output : TRUE | Side Effect : Who=tom, Age = 42
    
    - emp(tom,42) = emp(tim,Age)
    
    Output : FALSE | Side Effect Age= 42

3. Closures
    -  Define "closures"?

A useful thing that closures can do is keep track of internal state. A closure is created when:

The scope of some inner function refers to an outer scope's variables.

The inner function is passed around as a variable, carrying with it the inner scope and the outer scope.

    - In the following, when the `add` variable is initialized, what are the two parts of it contents?
    
 An anonymous function, and the variable counter

    - In the following, When the above `add` is created, then used 3 times, what is returns?             
```
 add = (function () {
    var counter = 0;
    return function () {return counter += 1;}
})();

add();
add();
add();
```

Returns 1, 2, 3

4. Type inference
     - It is claimed that languages that support type inference are less buggy. Why?

It requires the programmer to explicitly declaring the data type of an expression in the program, if the type doesn't match, it will throw an error.
     
     - Why might type inference be easier in Python than Java?

Python is a dynamically-typed language. Java is a statically-typed language. In a statically-typed language, the following sequence of statements (which binds an integer object, then a string object, to the name employeeName) is illegal. If employeeName had been declared to be an int, then the second statement would be illegal; if it had been declared to be a String, then the first statement would be illegal. But in a dynamically-typed language this sequence of statements is perfectly fine.


5. Folding
     - What is folding?

In functional programming, fold (also termed reduce, accumulate, aggregate, compress, or inject) refers to a family of higher-order functions that analyze a recursive data structure and through use of a given combining operation, recombine the results of recursively processing its constituent parts, building up a return value.

     - What does the following expression return? _foldl (+) 0 [1,2,3,4,5]_

15

6. Erlang
     - Nome one way Erlang is fundamentally different to Python.

Erlang is a functional programming language

     - Describe uses of Erlang in 2 industrial applications. What aspects of those applications lead to the
       use of Erlang?

Whatsapp and telephone switches. It can be up at all time, during the software patching period, if there's a call on the line, it will still be on the line during that period.

Erlang's main strength is support for concurrency. It has a small but powerful set of primitives to create processes and communicate among them.

Erlang provides language-level features for creating and managing processes with the aim of simplifying concurrent programming.


7. Heuristics
     - what is YAGNI? Describe an industrial scenario where YAGNI might save development costs.

"You aren't gonna need it". "Always implement things when you actually need them, never when you just foresee that you need them.


     - what is the rule of 3? Describe an industrial scenario where YAGNI might save development costs.

Rule of three is a code refactoring rule of thumb to decide when a replicated piece of code should be replaced by a new procedure. It states that the code can be copied once, but that when the same code is used three times, it should be extracted into a new procedure.

8. Patterns: Suppose you are working with a 3-tier architecture system for employee management. The system composed of  a database layer, business logic, and GUI. Many parts of codes are reused in this system. As an example: the database needs to know the valid ranges for `age` and so does the GUI.
     - What design pattern might be useful for the  business logic associated with this application? Give reasoning on behalf of your answer.


     
