# Tailwind CSS @apply Bug with Pseudo-elements and Responsive Modifiers

This repository demonstrates a bug in Tailwind CSS where the `@apply` directive fails to apply styles correctly to pseudo-elements (::before, ::after) when used with responsive modifiers.  The issue arises from the way Tailwind processes these class combinations, leading to an invalid CSS output.

## Bug Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the hover effect on the div does not apply the expected red background to the `::before` pseudo-element.

## Solution

The solution is to separate the responsive modifier and pseudo-element styles into different classes and apply them individually:

- Open `solution.html` to see how the bug is fixed.