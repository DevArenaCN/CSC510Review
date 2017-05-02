________________
# Review Ques 5



1. As precisely as you can (two lines each, at most), define the following.  Your definition should mention inputs,outputs and side-effects:
    - functions

???A function is a block of organized, reusable code that is used to perform a single, related action.

    - predictes

Predicate is a function that takes one element as input parameter and return either true or false. 

2. Assume a purely logic language where any word starting with upper case is an unbound variable.
   In that logical language what are the outputs and side-effects of the following:
    - emp(tim,42) = emp(Name,Age)
    - emp(Who,42)  =  emp(tom, Age)
    - emp(tom,42) = emp(tim,Age)



3. Closures
    -  Define "closures"?

A useful thing that closures can do is keep track of internal state. A closure is created when:

The scope of some inner function refers to an outer scope's variables.

The inner function is passed around as a variable, carrying with it the inner scope and the outer scope.

    - In the following, when the `add` variable is initialized, what are the two parts of it contents?

```
return counter += 1;

```

```
return function ()
```

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


     
     - Why might type inference be easier in Python than Java?
5. Folding
     - What is folding?
     - What does the following expression return? _foldl (+) 0 [1,2,3,4,5]_
6. Erlang
     - Nome one way Erlang is fundamentally different to Python.
     - Describe uses of Erlang in 2 industrial applications. What aspects of those applications lead to the
       use of Erlang?
7. Heuristics
     - what is YAGNI? Describe an industrial scenario where YAGNI might save development costs.
     - what is the  rule of 3? Describe an industrial scenario where YAGNI might save development costs.
8. Patterns: Suppose you are working with a 3-tier architecture system for employee management. The system composed of  a database layer, business logic, and GUI. Many parts of codes are reused in this system. As an example: the database needs to know the valid ranges for `age` and so does the GUI.
     - What design pattern might be useful for the  business logic associated with this application? Give reasoning on behalf of your answer.