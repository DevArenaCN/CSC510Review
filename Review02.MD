# Review 2 : Questions 2/14/2017

## Early lifecycle project planning:


1.    What are drawbacks of early requirement addressing?


2.    Define and distinguish unit, system and integration testing.

Unit testing is a software development process in which the smallest testable parts of an application, called units, are individually and independently scrutinized for proper operation.

System Testing is a level of the software testing where a complete and integrated software is tested.

Integration testing, also known as integration and testing (I&T), is a software development process which program units are combined and tested as groups in multiple ways. In this context, a unit is defined as the smallest testable part of an application.

3.    Describe two problems of underestimation effort.

Problem1: Uncertainty. We don't know how hard it will be to build software, until we build it.

Problem2: Better,Faster,Cheaper (pick any two). Deliver faster, spend less money? Prepare for more defects; Deliver faster with fewer defects? Stand by to spend lots more (e.g. on hyper-quality programmers); Fewer defects, spend less money? You'll need to reign in scope.

Problem3: Relucatance to Learn from Experience. When engineers fail to revise their beliefs, this leads to poor estimates.

4.    Describe two problems of underestimating effort.



5.    Boehm reports a certain shape in the cost-estimation uncertainty curve as a project moves from initial planning to final delivery
    - Draw that shape

![boehmEstimation](https://github.com/txt/se17/blob/master/img/boehmEstimation.png)

     - Why does the  shape change as the development continues?

Becuase at first, lack of maturity requires focus on risk and uncertainty issues, which makes it harder to estimate, later on, there are sufficient maturity to support detailed, high fidelity cost and schedule estimates, which makes it more accurate.

6. According to Brook's Law, why does adding more programmers to a late project make that project later?

(1) It takes some time for the people added to a project to become productive. (2) Communication overheads increase as the number of people increases. (3) Limited divisibility of tasks. Adding more people to a highly divisible task such as reaping a field by hand decreases the overall task duration (up to the point where additional workers get in each other's way). 



## Process planning:

0.    Draw the v-diagram. Divide into 
1.    Spiral models
       - What is the commit partition?
       - How is spriral connected to waterfall?
      - How is the spiral model _different_ to waterfall model?
      - How is the spiral model _the same_ as the waterfall model?
2.    When spiral model should not be practiced? Explain.
3.    Facebook ships many small  changes , very often.
      -  Which kind of s/w strategy method this is? 
4.    What are the phases of Test Driven Development cycle?
      -  List and explain three advantages of Test Driven Development?
      -  List and explain three disadvantages of Test Driven Development?

## Effort estimation

```python 
_  = None;  Coc2tunings = [[
#              vlow  low   nom   high  vhigh  xhigh   
# scale factors:
'Flex',        5.07, 4.05, 3.04, 2.03, 1.01,     _],[
'Pmat',        7.80, 6.24, 4.68, 3.12, 1.56,     _],[
'Prec',        6.20, 4.96, 3.72, 2.48, 1.24,     _],[
'Resl',        7.07, 5.65, 4.24, 2.83, 1.41,     _],[
'Team',        5.48, 4.38, 3.29, 2.19, 1.01,     _],[

# negative effort multipliers (more means faster)        
'acap',        1.42, 1.19, 1.00, 0.85, 0.71,    _],[
'aexp',        1.22, 1.10, 1.00, 0.88, 0.81,    _],[
'ltex',        1.20, 1.09, 1.00, 0.91, 0.84,    _],[
'pcap',        1.34, 1.15, 1.00, 0.88, 0.76,    _],[ 
'pcon',        1.29, 1.12, 1.00, 0.90, 0.81,    _],[
'plex',        1.19, 1.09, 1.00, 0.91, 0.85,    _],[
'sced',        1.43, 1.14, 1.00, 1.00, 1.00,    _],[ 
'site',        1.22, 1.09, 1.00, 0.93, 0.86, 0.80],[
'tool',        1.17, 1.09, 1.00, 0.90, 0.78,    _],[

# positive effort multipliers (more means slower)
'cplx',        0.73, 0.87, 1.00, 1.17, 1.34, 1.74],[
'data',           _, 0.90, 1.00, 1.14, 1.28,    _],[
'docu',        0.81, 0.91, 1.00, 1.11, 1.23,    _],[
'pvol',           _, 0.87, 1.00, 1.15, 1.30,    _],[
'rely',        0.82, 0.92, 1.00, 1.10, 1.26,    _],[
'ruse',           _, 0.95, 1.00, 1.07, 1.15, 1.24],[ 
'stor',           _,    _, 1.00, 1.05, 1.17, 1.46],[
'time',           _,    _, 1.00, 1.11, 1.29, 1.63]]
```

1.     COCOMO is a parametric effort estimation methods
      - What is the central intuition of the COCOMO equation?
      - Write down the COCOMO equation (hint: it should fit in half a line)
      - What are the for "P" of the COCOMO attributes? Give one example of each "P"
      - In COCOMO co-effecients are shown above, what is `acap` ? What happens to project development effort when it is increased? Why?
      - In COCOMO co-effecients are shown above, what is `cplx` ? What happens to project development effort when it is increased? Why?
      - From the above parameters, find how much faster a fully distributed system compared to a fully
centralized site. If needed, you may assume that the system has 100,000 lines of code.
2.    What is delphi based method? 
       - Why use it instead of COCOMO?
3.    "Planning poker" is  strategy is suitable for group discussion effort estimation environment
      -  Describe this approach plus one advantage and one disadvantage of using this method.
4.    What is no estimate method? When might it be s necessary? 
5.    Case base reasoning is called a non-parametric method.
      - Why? Hint: your answer will have to describe how it works
      - Give  2 advantages and disadvantages of CBR.
 
 
## Requirements

![](http://www.isa.us.es/sites/www.isa.us.es.featuremodelanalysis/files/images/MobilePhone.png)

1.   Consider the above feature model of a mobile phone. What features are allowed and forbidden in this diagram?
2.   Consider the design of a car. Every car has a body, transmission, and engine. 
     A car does not necessarily have a trailer. The engine may be powered with gasoline or with electricity or with both. Draw a feature model for car.
2.   A client has asked you to develop a word processor. 
     - Write two non functional requirements for this scenario.
       For each, list factors that make them easier or harder to fill
     - List two functional requirements
       For each, list factors that make them easier or harder to fill

