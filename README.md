# CSS Specificity Bug: Unexpected Inheritance

This repository demonstrates a subtle bug related to CSS specificity and inheritance.  The bug arises when a more specific selector fails to override inherited styles because of the way CSS specificity rules are calculated.

## Bug Description

The provided CSS code includes selectors that are intended to style nested elements. However, due to specificity issues, an expected style override does not occur. The text color unexpectedly inherits from a parent element, even though a seemingly more specific selector should take precedence.

## Reproduction Steps

1. Clone this repository.
2. Open `bug.css` and observe the CSS rules.
3. Create an HTML file to test the styles (see example in `index.html`).
4. Observe that the text color is green instead of purple. This demonstrates the unexpected inheritance.

## Solution

The solution involves modifying the CSS to ensure the desired style override is applied correctly by addressing the specificity issue. The solution is provided in `bugSolution.css`.

## Note

This issue highlights the importance of understanding CSS specificity when creating complex stylesheets.  It's crucial to be aware of how specificity affects inheritance to avoid unexpected styling behaviors.