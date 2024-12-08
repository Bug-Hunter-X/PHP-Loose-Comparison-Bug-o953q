# PHP Loose Comparison Bug

This repository demonstrates a common bug in PHP related to loose comparisons (`==`) between strings and integers. Loose comparisons do not check data type, which can lead to unexpected behavior.

## The Bug

The `bug.php` file contains code that demonstrates this issue. The script compares the string "0" to the integer 0 using a loose comparison (`==`).  Even though they represent different data types, PHP's loose comparison operator evaluates this comparison as true. This can cause unexpected behavior in your applications.

## The Solution

The `bugSolution.php` file provides a corrected version. It uses strict comparison (`===`) which checks both value and data type.  This ensures the comparison only evaluates to true if both operands are of the same type and have the same value. This makes the code more predictable and reliable. 

## How to Reproduce

1. Clone this repository.
2. Run `bug.php`. Observe the output. 
3. Run `bugSolution.php`. Observe the output and compare it to the output of `bug.php`
