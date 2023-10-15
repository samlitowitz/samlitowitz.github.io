---
layout: post
title:  "[WIP] Code Priority Hierarchy"
date:   2023-10-14 12:00:00 -0500
categories: programming wip
---

# Purpose

This document serves two purposes.
The first is to formalize the definitions of all items in the code priority hierarchy.
These terms are useful in many contexts beyond the code priority hierarchy and the definitions can provide a shared
basis of understanding to work from.
The second purpose is to provide a framework for developers which can guide their decisions for most cases.

# Code Priority Hierarchy

1. Correctness
2. Minimum Performance Requirements
3. Readability
4. Performance

The code priority hierarchy is an ordered list of attributes for an arbitrary piece of code.
The highest priority attribute is the first item in the list and the lowest priority attribute is the last item.
Attributes with a higher priority take precedence over attributes with a lower priority, e.g. a developer deciding
between readability and performance should prioritize readability.

## Correctness

Code is correct when, for any inputs and external state the code produces the correct output and external state.
Inputs and outputs are explicitly defined.
External states are implicitly defined by use in the code.
Code **MUST** satisfy correctness before any other attributes can be considered.

Corollary, dead code is code which does not affect the output or external state.

## Minimum Performance Requirements

The minimum performance requirements are an arbitrary set of metrics which the code must meet.
Code meets the minimum performance requirements when the code metrics conform to the minimum required metrics.

Corollary, if there are no minimum required metrics then this attribute is not a priority and should be ignored.

Corollary, if the metrics cannot be meaningfully measured then there are no minimum required metrics.

## Readability

Readability describes the ease (or difficulty) with which a developer can understand what the code is doing and why it
is being done.


For repeatable desirable outcomes, a developer **MUST** understand the code before using it or modifying it.


## Performance

Performance requirements are an arbitrary set of metrics which the code must meet.
Performance is the conformity of this codes metrics to the desired metrics.

Corollary, if there are no desired metrics then this attribute is not a priority and should be ignored.

Corollary, if the metrics cannot be meaningfully measured then there are no desired metrics.

# NOTES/WIP

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

