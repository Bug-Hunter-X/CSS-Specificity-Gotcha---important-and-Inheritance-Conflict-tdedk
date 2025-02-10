# CSS Specificity and Inheritance Conflict

This repository demonstrates an uncommon issue in CSS related to the interaction between specificity, inheritance, and the `!important` declaration.

## The Problem

The CSS code in `bug.css` shows a scenario where an `!important` declaration on a parent element does not override a more specific selector on the child element due to how inheritance works.  While `!important` generally wins in specificity conflicts, it only affects the direct styling of the element it is applied to; it does not 'cascade' down the inheritance chain.

## The Solution

The solution, provided in `bugSolution.css`, demonstrates how to correctly achieve the desired styling by adjusting the specificity to correctly target the inner paragraph or adding `!important` directly to the more specific selector.