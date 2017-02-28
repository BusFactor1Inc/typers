# typers

'typers' are variables that can be values or functions at runtime for Common Lisp. They are a conceptual idea that came to me years ago that I have finally realized during the production of my new music synthesizer 'waves'.  They are and simple and effective for the creation and composing of (time) varying signals or values.

The convention for typers is to use a trailing 'r' on a typer variable, such as 'countr' for a variable named 'count'.

There are currently 3 types of typer: 'booleanr', 'integerr' and 'floatr'.

Using a typer is done by wrapping any access of the variable in the corresponding type function:

```CL
(incf value (integerr count))
```

This convention (and requirement) to use typers offers a benefit of adding more type and variable usage information within the source code with little clutter, unlike most Common Lisp type declerations.

Currently, typers are implemented using functions, but I see a future of optimizations where macros will play a large part in their implementation roadmap.

--
Burton Samograd
2017
