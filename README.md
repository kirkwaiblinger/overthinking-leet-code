# Overthinking Leet Code

## Author
Kirk Waiblinger ([kirk.waiblinger@gmail.com](kirk.waiblinger@gmail.com))

## Overview

I recently started working on Leet Code problems in my spare time. I like to write thorough, generic solutions to the problems I work on. So, I'm making this public both for any interested parties to see, and to discourage myself from hacking away on the simpler problems.

For now, all problems are taken directly from [leetcode.com](https://leetcode.com/problemset/all/).

## Programming Approach

### Language Choice

For these types of problems, I find that Python is the easiest to use. For production code, I much prefer explicit variable declaration, block scoping, explicit typing, etc., that we get in other languages, since they make our code better for scalability and collaboration. On these kinds of quick problems, however, I find that Python gets us up and running very quickly, and has an enormously useful standard library.

### Generic Solutions

Many problems, particularly those to do with iteration, ask us to find maybe the 2nd or 3rd element satisfying some condition. I find that a simple recursive approach typically gets us what we need for a constant hard-coded n. However, I prefer to write generic code that lazily yields all elements in order, and chooses to consume however many the problem asks for. For instance, see the binary tree cameras problem (#812).

For me, the easiest and most readable way to achieve this tends to be by using generator functions to create iterables, and consuming only what we need from them. Python, in particular, has excellent syntactical support for generators and for the higher-order order functions that help us manipulate them.


## Miscellany

- The leetcode.com problems are labelled with their difficulty _according to leetcode.com_. I may make a comment if I disagree significantly with that difficulty evaluation.