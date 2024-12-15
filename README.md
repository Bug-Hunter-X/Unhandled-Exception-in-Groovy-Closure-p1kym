# Unhandled Exception in Groovy Closure
This example demonstrates a common issue in Groovy when exceptions are thrown within closures.  The exception in the closure is not caught by the calling method, leading to abrupt termination of the program.

## Problem:
The `methodWithClosure` function calls a closure. If the closure throws an exception, the program will crash without any proper handling of the exception within the calling method.

## Solution:
The solution involves using a `try-catch` block within `methodWithClosure` to handle exceptions that might be thrown by the closure.