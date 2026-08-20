# Required and Optional Parameters

Some function parameters are required every time the function is called. Others can be optional and do not need to be provided every time. In many languages, this is achieved by giving them a default value. If the function call does not provide an optional argument, the default value is used.

# Conceptual Rule

In general terms, a function can be designed so that:

* Required arguments must always be supplied.
* Optional arguments have sensible default values.
* Supplying an argument replaces the default for that call only.

# Pseudocode Example

The following example shows a function which adds together the variables `x` and `y`, but also has an optional argument `z` which defaults to 0. The function will sum and return all three variables.

```
FUNCTION add(x, y, z=0) // Arguments x and y are required, z is optional with default value 0
    RETURN x + y + z
END FUNCTION

PRINT add(5, 10)  // Returns 15, using default z=0
PRINT add(5, 10, 15)  // Returns 30, using provided z=15
```

# Why default Argument Values are useful

Default arguments make common function calls shorter while still allowing advanced behaviour when needed. They also help communicate intended behaviour by making standard choices explicit in the function definition.
