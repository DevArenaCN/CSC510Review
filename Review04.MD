# Review Ques 4

1. What one thing we should be expect in:
       - a poorly architectured system?



       - a well architectured  system?

Something that lets you work alone half the time, team members can be productive in isolation, but know when they need to talk to others.

2. Package switching network (PSN):
       - Define the components of a PSN

Nodes, hosts, packets.

       - What other architecture was package switching designed to replace?

Centralized and decentralized.

       - Why was an advantage of that other architecture?



       - What feature of PSN make it attractive as an alternate architeture?

Won't jammed up if one of the hosts are experiencing heavy traffic.

3. Blackboard architecutures:
       - Define the components of a blackboard architecture;

Blackboard: global database and knowledge source: logically independent sources of knowledge

       - For which projects are  blackboard architectures are ideal?  

 Each knowledge source updates the blackboard with a partial solution when its internal constraints match the blackboard state. In this way, the specialists work together to solve the problem. The blackboard model was originally designed as a way to handle complex, ill-defined problems, where the solution is the sum of its parts.

4. Pipe and Fiter:
       - Describe the components of a pipe and filter architecture.

a pipeline consists of a chain of processing elements (processes, threads, coroutines, functions, etc.), arranged so that the output of each element is the input of the next; Usually some amount of buffering is provided between consecutive elements. The information that flows in these pipelines is often a stream of records, bytes or bits, and the elements of a pipeline may be called filters.

       -  Give an example of a commonly used system that makes extensive use
         of pipe and filter

Unix

       - Explain one advantage of pipe and filter

Simplicity – Allows designer to understand overall input/output behavior of a system in terms of individual filters.

Concurrent Execution –Each filter can be implemented as a separate task and be executed in parallel with other filters.


       - Explain one disadvantage of pipe and filter

Interactive transformations are difficult – Filters being independent entities designer has to think of each filter as providing a complete transformation of input data to output data.

No filter cooperation.

Performance – may force a lowest common denominator on data transmission

5. Layered architectures:
       - What is "LAMP" and why is it an example of a layered architecture?

LAMP = Linux apache mysql php (python). Segregates functionality into separate segments in much the same way as the layered style, but with each segment being a tier located on a physically separate computer.

       - Explain one advantage of a layered architecture.

Abstraction. Layered architecture abstracts the view of the system as whole while providing enough detail to understand the roles and responsibilities of individual layers and the relationship between them.

       - Explain one disadvantage of pipe and filter

Interactive transformations are difficult – Filters being independent entities designer has to think of each filter as providing a complete transformation of input data to output data.

       - What is "MEAN" and why is it sometimes called a "leaky layered" architecture?

MEAN = MongoDb, Express, Angular, NodeJS. Everything is done in JavaScript, and there's no OS involved.

       - Why is MEAN replacing LAMP in certain fast-paced organizations?
One language (JavaScript), one language up and down the stack (javascript) so (1) faster integrated testing; and (2) faster invention of new patterns.; NoSQL database, easy to scale.


6. CRUD:
       - What is the CRUD pattern?

In computer programming, create, read, update and delete (as an acronym CRUD or possibly a backronym) (Sometimes called SCRUD with an "S" for Search) are the four basic functions of persistent storage.
Sometimes CRUD is expanded with the words retrieve instead of read, modify instead of update, or destroy instead of delete. It is also sometimes used to describe user interface conventions that facilitate viewing, searching, and changing information; often using computer-based forms and reports.

       - Give two example where CRUD pattern is used. 

Databases
Distributed database services
RESTful interfaces


7. In Windows
    machine if you open one folder in two different views, rename folder in
    one view automatically renames the other.
       - What type of architecture is this?  

Subject-Observer

       - Describe different components of this architecture with respect to the above example.


       
