# Tailwind CSS Flexbox Overflow Issue

This repository demonstrates a common issue encountered when using Tailwind CSS flexbox layouts: unexpected column stacking when content overflows the assigned width.  The problem arises when the content within a flexbox item exceeds the width allocated by Tailwind's fractional width classes (e.g., `w-1/2`).

## Problem
The provided `bug.html` file shows a simple flexbox layout with two columns.  If the content in either column becomes too wide, the columns will unexpectedly stack vertically instead of remaining side-by-side.

## Solution
The `solution.html` file demonstrates several solutions to address this issue:

* **Using `flex-shrink-0`:** This prevents the columns from shrinking below their initial size, forcing them to remain side-by-side even with overflowing content.
* **Adding `overflow-x: auto;`:** This introduces horizontal scrollbars to accommodate overflowing content, allowing the columns to remain in a row.
* **Responsive design approaches:** Use different width classes for different screen sizes or adjust the content to fit within the allocated width.

Choose the solution that best fits your specific requirements and design goals.