# typers

'typers' are variables that can be values or functions at runtime for Common Lisp

The convention is to use a trailing 'r' on a typer variable, such as 'countr' for a variable named 'count' that happens to be a typer.

There are currently 3 types of typer: 'booleanr', 'integerr' and 'floatr'.

Using a typer is done by wrapping any access of the variable in the corresponding type function:

```CL
(integerr count)
```

This convention (and requirement) to use typers offers a benefit of adding more type information within the source code.
