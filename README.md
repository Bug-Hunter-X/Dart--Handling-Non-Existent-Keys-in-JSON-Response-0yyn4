# Dart: Handling Non-Existent Keys in JSON Response

This repository demonstrates a common error in Dart when working with JSON responses: attempting to access a key that doesn't exist in the JSON data.  The `bug.dart` file shows the problematic code, while `bugSolution.dart` provides a solution.

The error occurs because the code assumes the JSON response will always contain a key named `nonExistentKey`. If the API response doesn't include this key, accessing it will result in an exception.

The solution involves checking for the key's existence before accessing it using `jsonResponse.containsKey('nonExistentKey')` to avoid runtime errors.
