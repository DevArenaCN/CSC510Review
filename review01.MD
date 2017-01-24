# Review Questions 1/19/2017

Test-drven Development

-    According to Kent Beck, why are feedback loops in software development so important?

     + Feedback loops can provide customer satisfaction by rapid, continuous delivery of useful software.

-    When building tests, what is a _mock_ and why are such mocks important?

     + _mock_ is a fake function that mimic the behavior of the real one, so that other functions can run even without the function being declared.

-    What is red green test?

     + **RED:** 
     Start by thinking of a behavior you want the software to have which could be implemented by a few lines of code (fewer thanfive is a good target). Then write a test (also only a few lines of code) that will fail unless that behavior is present. Focus on:
      + The class behavior and its public interface - not how to implement the internals of the class.
      + The class user, not the class implementer - you may need to write the first few tests with class and method names that do not yet exist. Run the test suite, and watch the new test should fail. If the test either does not fail or fails in a different way than you intended, make the necessary fixes.
+ **GREEN:** Write just enough code to get the test to pass. Focus on:
      + Getting something to work
      + Simplest possible implementation, rather than the most elegant solution (even hard-coded values are okay).
      + Reverting to known good code if the test continues to fail
      + If after a few attempts you can't make the test pass, consider starting over with a different test, possibly employing even less code. 

-    What are advantages and disadvantages of test-driven development?

     ### Advantage

     + Over-engineering. I have a tendency to "throw in" functionality I "know" I'm "going to need". Making one red test green (along with the list of future tests) helps me implement just enough. I need to find a new way to stay focused.
     + API feedback. Get quick feedback about my API decisions.
     + Logic errors. Catches pesky errors.
     + Documentation. Communicate how I expect APIs to be used and to record what I was thinking during development.
     + Feeling overwhelmed. With TDD, even if I couldn't imagine an implementation I could almost always figure out how to write a test (finding the next "step up the mountain").
     + Separate interface from implementation thinking. I have a tendency to pollute API design decisions with implementation speculation. TDD separates the two levels of thinking while still providing rapid feedback between them.
     + Agreement. A way to be precise with a programming partner about what problem I'm solving.
     + Anxiety. TDD gives me an instantaneous "Is Everything Okay?" button.

### Disadvantages


   + Notes that _unit tests_ are very small while _function tests_ (aka _system tests_) are much larger, much more complex.
    + Much slower to run, not the kind of thing to give you instant feedback.
     + "Tests might be more complex than the actual code."
     + "Unit tests are unlikely to test more than one
      trillionth of the functionality of any given method in a
       reasonable testing cycle. Get over it."
     + "If you find your testers splitting up
      functions to support the testing process,
      you’re destroying your system architecture and
      code comprehension along with it. **Test at a coarser level of granularity.**"
     + "Tests should be designed with great care. Business
      people, rather than programmers, should design most
       functional tests. Unit tests should be limited to those that
       can be held up against some “third-party” success criteria."
     + "If you have a large unit test mass, evaluate the feedback
      loops in your development process. Integrate code more
      frequently; reduce the build and integration times; cut the
      unit tests and go more for integration testing. "

Process models

-    Describe the four parts of the v-diagrams?
     -     Which part(s) of the v-diagram takes most time?
     -     Which part(s) take least time?
-    Name, in order, at least four stages of waterfall model? 
     -     Why is it called waterfall model?
-    Give an example application where the waterfall model might be suitable for. 
-    What are the  major disadvantages of the waterfall model?
-    Describe the agile model. 
     -     What are its key differences compared to waterfall model?
     -     What are some potential disadvantes of agile?
-    Describe  DevOps? Why it is called DevOps?


Surveys

-    An individual in a survey has three rights.  In 2 lines (each) describe two survey procedures: one that maintains and one that violates
     -   a subject’s right not to participate.
     -   a subject’s right to privacy.
     -   a subject’s right to be forgotten.
-    For each of the following, use 2-5 lines to define and describe:
     -  Semi-structured or structured interviews
     -  Questionaires
     -  Focus groups
     -  Think aloud
     -  Data analysis (using data mining)
-    Pick any two of the above survery methods  and describe how one can be **better** than the other.
-    Pick any two of the above survey methods and describe one can be **worse** than the other.


Stakeholders

-   Who are stake holders?
-   What is non functional requirement of stakeholders?
-   Assume you are assigned to develop a website of CSC department. Describe different solution for different stakeholders.
-   What is feature option? Assume you have to design the architecture of a mobile phone. What will be the feature options in this context?
