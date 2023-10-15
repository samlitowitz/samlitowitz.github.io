---
layout: post
title:  "[WIP] Code Priority Hierarchy"
date:   2023-10-14 12:00:00 -0500
categories: programming wip
---

# Purpose

1. formalize definitions
1. formalize priority

This document serves two purposes.
The first is to formalize the definitions of all items in the code priority hierarchy.
These terms are useful in many contexts beyond the code priority hierarchy and the definitions can provide a shared
basis of understanding to work from.
The second purpose is to provide a framework for developers which can guide their decisions for most cases.

~The second purpose is to define a set of prioritized attributes for code which can be used in most cases to provide developers a framework~

# Code Priority Hierarchy

[TODO]: <> (where do I put the actual list for maximum understanding/readability/context?)

1. Correctness
2. Minimum Performance Requirements
3. Readability
4. Performance

The code priority hierarchy is an ordered list of attributes for an arbitrary piece of code.
The highest priority attribute is the first item in the list and the lowest priority attribute is the last item.
Attributes with a higher priority take precedence over attributes with a lower priority, e.g. a developer deciding
between readability and performance should prioritize readability.

[TODO]: <> (why does this matter???)

[TODO]: <> (purpose!)



1. Correctness

   For any inputs and external state the code produces the correct output and external state.
   Corollary, dead code is code which does not affect the output or external state.

2. Minimum Performance Requirements, Readability, Performance

Readability is the ability for a developer (including later you) to understand what you are doing and why.
Performance is the conformity of this codes metrics when executing to acceptable metrics.

It is almost always better to trade performance (within the accepted tolerances) for readability.

Most other "rules" exist to promote the above priorities.
Example/case study: Don't Repeat Yourself (DRY)

