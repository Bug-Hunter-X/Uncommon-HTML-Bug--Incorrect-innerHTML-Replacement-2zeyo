# Uncommon HTML Bug: Incorrect innerHTML Replacement

This repository demonstrates a subtle bug in HTML that occurs when attempting to replace the innerHTML of an element using a variable without proper string concatenation. The bug leads to unexpected behavior.

## Bug Description
The bug arises from an incorrect attempt to dynamically update the content of a div element using javascript. When the javascript code tries to assign a variable directly to innerHTML, the script might produce unexpected behavior or errors. This error occurs particularly when string values are not concatenated correctly to assign the variable to the innerHTML attribute of the html tag.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe that the text within the div element is not replaced as expected.

## Solution
The solution involves correctly concatenating the variable containing the new text using the + operator before assigning the string to the innerHTML attribute of the tag.  Ensure that values are stringified before assigning to the innerHTML attribute.

## Files
* `bug.html`: The HTML file containing the bug.
* `bugSolution.html`: The HTML file with the corrected code.