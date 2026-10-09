# Week 6 Assignment: Python Exception Handling

**Author:** Farah  
**Date:** October 9, 2026  

## File Descriptions
* `safe_tools.py`: A collection of defensive helper functions that utilize `try / except` statements to safely process mathematical calculations, type conversions, and key lookups without crashing.

---

## Assignment Analysis Question

### Why can a standard `if` check not catch `"abc"` on its own when converting to an integer?
An `if` statement can only evaluate Boolean logical conditions or explicit string values; it lacks the built-in capability to analyze whether an arbitrary sequence of letters can successfully be transformed into base-10 numerical data blocks. 

If you pass `"abc"` into an `if` block, checking its value directly does not prevent a crash. Python requires an explicit `try / except` statement to trap the runtime `ValueError` raised by the `int()` constructor when it encounters unparseable non-numeric characters.
