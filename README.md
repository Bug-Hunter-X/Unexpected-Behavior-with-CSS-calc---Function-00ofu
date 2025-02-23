# Unexpected Behavior with CSS calc() Function

This repository demonstrates a common yet subtle error involving the `calc()` function in CSS.  The issue arises when using `calc()` to calculate a width (or other dimension) relative to a percentage, but the parent container doesn't have a explicitly defined width.  This can lead to unexpected results, as the calculation relies on the parent's width being known.

The `bug.css` file showcases the problematic code, while `bugSolution.css` provides a solution.

## Bug Description
The `calc()` function, while powerful, requires careful consideration of the context in which it's used.  If the parent container lacks a defined width, the calculation based on percentage may fail, leading to an element's width not being rendered as expected.