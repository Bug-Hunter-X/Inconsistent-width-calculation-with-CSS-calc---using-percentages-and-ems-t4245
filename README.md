# Inconsistent Width Calculation with CSS calc() using Percentages and Ems

This repository demonstrates an issue with unexpected behavior when using the `calc()` function in CSS with a mix of percentage and `em` units. The problem lies in the potential for inconsistent calculations across different browsers and viewport sizes, leading to unpredictable layout.

## Problem Description

The intention is to make an element slightly smaller than 50% of its parent's width. However, the interaction between percentage and absolute units within the `calc()` function introduces complexities, which may lead to layout differences across different browser implementations.

## Solution

The best approach is to avoid mixing percentage and absolute units directly within the `calc()` function where possible.  Consider using a more consistent unit or adjusting the approach to layout.  The solution provided uses viewport units (vw) for a consistent relative unit.