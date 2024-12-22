# Uncommon HTML Bug: DOM Element Manipulation Before Load

This repository demonstrates a subtle bug in HTML where JavaScript attempts to manipulate a DOM element before the element has fully loaded into the DOM.  This can lead to unexpected behavior, often with no obvious error messages.

The bug is caused by the script attempting to access and modify the `myDiv` element before it exists in the DOM tree. This is a race condition. The solution demonstrates how to ensure the script only runs after the DOM is fully loaded using the `DOMContentLoaded` event.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe that the text within the `div` element is not hidden; the script fails silently.
4. Open `solution.html` to see the corrected code.
