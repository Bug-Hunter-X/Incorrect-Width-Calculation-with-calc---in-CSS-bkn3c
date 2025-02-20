# Incorrect Width Calculation with calc() in CSS

This repository demonstrates a common issue encountered when using the `calc()` function in CSS to calculate widths.  The problem arises when subtracting a fixed value (pixels) from a percentage value.

The `bug.css` file contains the problematic CSS code.  The `bugSolution.css` file offers a solution that provides the expected result.

## Problem
The `calc(100% - 50px)` calculation, while seemingly straightforward, can lead to unexpected results depending on the parent element's width and the browser's rendering engine. In certain situations, the element's actual width may be significantly less than the calculated value.

## Solution
One possible solution is to define a more explicit calculation, potentially using a different approach or explicitly setting the width to `450px` if that is the intended width. Alternatively, using flexible box model or grid layout can more easily handle such calculations.