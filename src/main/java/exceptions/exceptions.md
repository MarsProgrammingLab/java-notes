## Exceptions
- Exceptions interrupt the normal execution of a program.

## Exception handling
- Exception handling deals with exceptions without stopping the entire program.
- Works with both checked and unchecked exceptions.
- An exception can be handled in the method where it occurs or in the calling method.
- Three keywords for handling exceptions: try, catch, finally
- Try/catch template:

	try {
    	// code that may throw an exception
	} catch (Exception e) {
    	// code for handling the exception
	}
	
- The try block wraps the code that may throw an exception while the catch block handles this exception in case it occurs, also allowing us to get some information about it. It is possible to use several handlers to provide different scenarios for different types of exceptions. 

- There's an optional finally block that is always executed. Its main feature is that it executes even if we fail to handle an exception at all.

- Any object of the `Throwable` class and all its subclasses can be thrown using the throw statement. The general form of the statement consists of the `throw` keyword and an object to be thrown.

- Example using object of `RuntimeException`:
	
	public class Main {
	    public static void main(String args[]) {
	        RuntimeException exception = new RuntimeException("Something's bad.");
	        throw exception;
	    }
	}

- Common practice to create and throw exception in single line
- Example using instance of `Throwable`:
	
	throw new Throwable("Something's bad.");

