# Tailwind CSS @apply Bug with Pseudo-selectors

This repository demonstrates a bug in Tailwind CSS where the `@apply` directive fails to apply styles when used with pseudo-selectors like `:hover`, `:focus`, etc.

## Bug Description

The `@apply` directive in Tailwind CSS is designed to apply the styles of a pre-defined class to another element. However, when using `@apply` with a class containing a pseudo-selector, the styles of the pseudo-selector are not applied.  This leads to unexpected styling issues.

## Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the hover effect is not applied to the button.

## Solution

The solution is to avoid using `@apply` with classes containing pseudo-selectors. Instead, use the pseudo-selectors directly in the class names applied to the element.

See `bugSolution.html` for the corrected code.