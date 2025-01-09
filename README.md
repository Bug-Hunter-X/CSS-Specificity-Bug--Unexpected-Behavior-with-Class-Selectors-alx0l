# CSS Specificity Bug

This repository demonstrates an uncommon bug related to CSS selector specificity.  The issue arises from a misunderstanding of how CSS resolves conflicting styles based on selector specificity. 

## The Problem

The `bug.css` file contains CSS rules that result in an unexpected outcome. The `.item.special` class selector overrides `.container .item.special`, even though the latter appears more specific due to the additional parent container selector. This is due to specificity rules prioritizing selectors with more class or ID selectors. 

## The Solution

The `bugSolution.css` file offers a solution to this problem by using the `!important` flag to ensure that the correct style is applied. Please note that using `!important` should be avoided unless absolutely necessary.