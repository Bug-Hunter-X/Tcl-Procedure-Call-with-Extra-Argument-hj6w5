# Tcl Procedure Call with Extra Argument

This repository demonstrates a common error in Tcl: calling a procedure with more arguments than it is defined to accept.  The `bug.tcl` file shows the erroneous code, while `bugSolution.tcl` provides the corrected version.

The issue arises from passing three arguments to `myproc`, which only expects two. Tcl handles this silently (it just ignores the extra arguments), leading to potentially confusing behavior if you're not aware of this. 

The solution highlights the importance of carefully matching the number of arguments passed to a procedure with the number it's designed to receive.  Using variable-length argument lists (`args`) when necessary, provides more flexibility in procedure definition.