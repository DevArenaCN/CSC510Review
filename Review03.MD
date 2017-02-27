# Review Ques 3 02/14/2017

## Requirement Analysis:

1)   Defend the following statements

       - Before building any software, it is wise to spend much time collecting details requirements docs.

Ideally, we look before we leap so that we can find the best ways to do proceed (and we don't get it wrong).
       
      - Requirements engineering is a waste of time

Experience tells you more than excessive initial analysis, recent research says requirements are an illusion.

2)    What is commit partition? What is commit partition strategy in spiral model?




3)    Defend the following statemetns
        - Reuse is the key to productivity



        - Reuse is dangerous 


        
4)    What are the arguments for and against pushing small codes to review?

Ship small diffs, and stand a snowball’s chance of inspecting them for correctness; because code isn’t correct until it’s running production; because the last thing you changed is probably setting those fires. code review! smaller = faster = more thorough!


Against:  Limiting the amount of code you push is going to block progress, unless you can simultaneously increase the rate of pushing code. This is not as easy as it sounds, and it will shift the focus of your developer tooling budget in the direction of software built with this goal in mind.  You don’t need elaborate Git release rituals. Ceremony such as tagging releases gets to feel like a waste of time once you are releasing many times per day.

______________________________________________
 
  ##Visual Notations for Programming:
 
5)    Write two advantages of state chart. 

6)  When state chart is not recommended?

7 )  Draw a state chart for the following states and transitions:
struct transition state_transitions [] = {
{entry, ok, foo},
{entry, fail, end},
{foo, ok, bar},
{foo, fail, end},
{foo, repeat, foo},
{bar, ok, end},
{bar, fail, end},
{bar, repeat, foo}};
  

8) Write three differences between SQL and No-SQL.

9)    Suppose you have three tables in database: University, Subject and Student. What are insert, update and delete anomalies in this context?

10)    How ER based model solves different anomalies for the above scenario? Explain.

11)    Why doe some people claim ER is not suitable for agile development?

12)    What state chart and ER based models have in common?

13)    What is compartmental model? Give a small example of using this model for a grocery shop supply chain from warehouse to supermarket shelves.

14)    What are the limitations of compartmental model?
