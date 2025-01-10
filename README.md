# CSS `calc()` Function Inconsistency

This repository demonstrates an uncommon issue related to the CSS `calc()` function.  The problem occurs when the `calc()` function is used to determine the width of an element whose parent doesn't have an explicitly defined width.

Some browsers may interpret `100%` within the `calc()` function relative to the viewport, leading to inconsistent results across different browsers. Others might use the nearest ancestor with a defined width, creating unpredictable behavior. The `bug.css` file showcases the problematic CSS rule.

The solution, provided in `bugSolution.css`, involves ensuring the parent element has a defined width, thus providing a reliable baseline for the `calc()` function.