# Uncommon HTML Bug: Unexpected innerHTML behavior

This repository demonstrates an uncommon bug related to the use of `innerHTML` in HTML/Javascript.  Specifically, attempting to set `innerHTML` to a non-string value can lead to unexpected results, such as an empty or unpopulated div.

## Bug Description
The bug lies in the improper usage of `innerHTML`.  The `innerHTML` property expects a string value. When a non-string is passed, the browser attempts to convert it. This conversion can lead to unexpected outcomes.

## Bug Reproduction
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe that the `div` with the id "myDiv" does not display the numerical value as expected, but is instead empty or contains unexpected output.

## Solution
The solution is to always pass a string value to `innerHTML`, either directly or by explicitly converting the non-string value using the `toString()` method.
