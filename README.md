# Lua pairs iterator unexpected behavior
This repository demonstrates an uncommon bug in Lua related to the `pairs` iterator and table modification during iteration.

The `bug.lua` file contains code that recursively iterates through a nested table using `pairs`. If the table's structure is modified during iteration, `pairs` might not visit all elements, leading to unexpected results.

The `bugSolution.lua` file provides a workaround using a copy of the table to prevent modification during iteration.