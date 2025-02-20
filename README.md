# Tailwind CSS `@apply` Directive Error: Referencing Undefined or Misspelled Class

This repository demonstrates a common yet often overlooked error in Tailwind CSS when using the `@apply` directive within custom directives.  The error occurs when the `@apply` directive attempts to use a class that is either undefined, misspelled, or has a naming conflict.

## The Bug
The `bug.css` file contains an example of this error. A custom directive `.custom-button` uses `@apply` to apply multiple Tailwind classes. However, one or more of the classes might be misspelled or not defined in your `tailwind.config.js` leading to unexpected styling issues.

## The Solution
The `bugSolution.css` file demonstrates how to fix this bug.  The solution involves carefully reviewing the Tailwind classes used within the `@apply` directive, correcting any misspellings, and ensuring that all referenced classes are correctly defined in your Tailwind configuration.