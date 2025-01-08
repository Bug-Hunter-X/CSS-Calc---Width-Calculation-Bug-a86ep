# CSS Calc() Width Calculation Bug

This repository demonstrates a bug related to the use of `calc()` for width calculation in CSS.  Some browsers may not correctly interpret the calculation `calc(50% - 10px)`, resulting in unexpected layout issues.

The `bug.css` file contains the problematic CSS, while `bugSolution.css` demonstrates a workaround to resolve the issue.

## Bug Description
The CSS uses `calc()` to calculate the width of a div, subtracting 10px from 50% of the container's width. This leads to inconsistent rendering across different browsers.

## Solution
The suggested solution is to avoid using `calc()` for complex percentage-based width calculations, which can result in inconsistencies in some browsers.  Alternatively, consider adding a wrapper to manage the element's positioning more precisely.