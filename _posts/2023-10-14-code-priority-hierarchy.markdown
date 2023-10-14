---
layout: post
title:  "[WIP] Code Priority Hierarchy"
date:   2023-10-14 12:00:00 -0500
categories: programming wip
---

1. Correctness

    For any inputs and external state the code produces the correct output and external state.
    Corollary, dead code is code which does not affect the output or external state.

2. Readability, Performance

Readability is the ability for a developer (including later you) to understand what you are doing and why.
Performance is the conformity of this codes metrics when executing to acceptable metrics.

It is almost always better to trade performance (within the accepted tolerances) for readability.

Most other "rules" exist to promote the above priorities.
Example/case study: Don't Repeat Yourself (DRY)

