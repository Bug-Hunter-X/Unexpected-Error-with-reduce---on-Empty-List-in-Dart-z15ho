# Dart reduce() on Empty List Error

This example demonstrates an uncommon error in Dart when using the `reduce()` method with an empty list. The `reduce()` method requires at least one element in the list; otherwise, it throws an `UnsupportedError: Empty list` exception.  This behavior is not always intuitive and can be a source of difficult-to-debug runtime issues.

The `bug.dart` file shows the error, and the `bugSolution.dart` provides a solution using an optional check for an empty list.

## Solution
The solution involves checking the list's length before calling `reduce()`.  If the list is empty, a default value is returned, preventing the error.