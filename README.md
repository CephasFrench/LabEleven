Tasks to answer in your own README.md that you submit on Canvas:

1.  See logger.log, why is it different from the log to console?
    1. ANSWER: The reason why the logger.log file is different from the log in the console is because the text shown in the console is from the system out and the log information is from Logger class.
1.  Where does this line come from? FINER org.junit.jupiter.engine.execution.ConditionEvaluator logResult Evaluation of condition [org.junit.jupiter.engine.extension.DisabledCondition] resulted in: ConditionEvaluationResult [enabled = true, reason = '@Disabled is not present']
    1. ANSWER: This line comes from the logger.log file and sees if the tests will run or not.
1.  What does Assertions.assertThrows do?
    1. ANSWER: The Assertion.assertThrows is a JUnit Jupiter method for asserting a piece of particular code that throws an exception. If an exception is thrown inside the Lambda expression then the method will assert.
1.  See TimerException and there are 3 questions
    1.  What is serialVersionUID and why do we need it? (please read on Internet)
        1. ANSWER: SerialVersionUID is used for verification for when the class is Serialized and deserialized over a byte stream. This helps keep compatibility between the class versions as the local and serialized versions can be compared to see if they are compatible.
    2.  Why do we need to override constructors?
        1. ANSWER: we need to override the constructors so that we can call the correct constructors of the super class based of the arguments passed to the constructor.
    3.  Why we did not override other Exception methods?	
        1. ANSWER: We do not need to override other methods because the default actions of these methods are sufficient for our needs.
1.  The Timer.java has a static block static {}, what does it do? (determine when called by debugger)
    1. ANSWER: The static block static {} Initializes static variables like the logger. This block of code is run when the class is loaded on the JVM before any instance of the class or static member is accessed. This insures that the block is only run once.
1.  What is README.md file format how is it related to bitbucket? (https://confluence.atlassian.com/bitbucketserver/markdown-syntax-guide-776639995.html)
    1. ANSWER: The README is formatted in Markdown. This is related to bitbucket because bitbucket uses Markdown for their README files.
1.  Why is the test failing? what do we need to change in Timer? (fix that all tests pass and describe the issue)
    1. ANSWER: The test is failing because timeNow was null and was not set before the exception was thrown. To fix this set time before the exception check.
1.  What is the actual issue here, what is the sequence of Exceptions and handlers (debug)
    1. ANSWER: The real issue is that once the exception is thrown, the program goes to the final block of the code skipping where the timeNow was set.
1.  Make a printScreen of your eclipse JUnit5 plugin run (JUnit window at the bottom panel) 
1.  Make a printScreen of your eclipse Maven test run, with console
1.  What category of Exceptions is TimerException and what is NullPointerException
    1. ANSWER: The category is EException, which needs to be handled in a try catch block. NullPointerException is a runtime exception.
1.  Push the updated/fixed source code to your own repository.