**Exception:** Exception is an unexpected event that disrupts the normal flow of program.

**Exception vs Error:**

* Exception is a recoverable problem caused by program logic and can be handled using try-catch. 
&nbsp;  Example: Arithmetic exception (/ by 0).

* Error is a serious problem caused by the system or JVM and usually cannot be handled. 
&nbsp;  Example: Stack overflow error.

Object class (main class)--> Throwable class (handles all errors and exceptions) -->  Error & Exception classes.
Exception: Checked & Unchecked Exceptions

**Checked Exception:** if you get an exception during compile-time, it will be a checked exception.
**Unchecked Exception:** if you get an exception during run-time, it will be an unchecked exception.

Some keywords related to exception handling in Java:

**1. try:** try block contains code that might cause an exception.

**2. catch:** if an exception happens inside the try block, the catch block handles it.

**3. finally:** finally block always executes, whether an error happens or not. It is usually used for cleanup (like closing files or database connections).

**4. throw:** throw keyword is used to explicitly create and send an exception. It is used inside a method. It is used to throw a single exception.

**5. throws:** throws keyword is used to declare exceptions. It is used in method declaration. it can declare multiple exceptions.



**throw vs throws:**

* throw is used to explicitly throw an exception inside a method.
* throws is used to declare exceptions in the method signature.

**Note:** 

\# There can be multiple catch blocks for one try block but the order matters: parent category cannot come before the child category --> "Catch(ArithmeticException e)" should come before "Catch(Exception e)". Otherwise you get a compile-time exception something like "Exception is already caught".

\# The finally block is optional and there can only be one finally block.

\# You can also create your own exceptions by creating a class that extends Exception class.








