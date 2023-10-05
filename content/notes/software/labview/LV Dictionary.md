---
title: "LV Dictionary"
feed: show
date: "2023-10-05"
tags: 
---

Some notes about random [[notes/software/labview/LabVIEW|LabVIEW]] concepts 

## Channel Wires
- can be used to visually understand sending objects through wires
- channels are dynamically created when loaded, and then compiled. This is in contrast to the typical compilation for LabVIEW which is compiled upon load
- good for visualization
- Some concepts: channel queue, chunking size

## Inline VIs

From the LV Help:
### SubVI Overhead

When you call a subVI, there is a certain amount of overhead associated with the call. This overhead is fairly small (on the order of tens of microseconds), especially in comparison to I/O overhead and display overhead, which can range from milliseconds to tens of milliseconds. However, this overhead can add up in some cases. For example, if you call a subVI 10,000 times in a loop, this overhead could significantly affect execution speed. In this case, you might want to consider embedding the loop in the subVI.

Another way to minimize subVI overhead is to turn subVIs into subroutines by selecting **Execution** from the **Category** pull-down menu in the VI Properties dialog box and then selecting **subroutine** from the **Priority** pull-down menu. However, there are some trade-offs. Subroutines cannot display front panel data, call timing or dialog box functions, or multitask with other VIs. Subroutines are generally most appropriate for VIs that do not require user interaction and are short, frequently executed tasks.

A third way to minimize subVI overhead is to inline subVIs into their calling VIs. When you inline a subVI, LabVIEW inserts the compiled code of the subVI into the compiled code of the calling VI. If you then make changes to the subVI, LabVIEW recompiles all calling VIs of that subVI to include those changes. Essentially, inlining a subVI removes the need to call the subVI at run time. Instead, LabVIEW executes the subVI code inside the compiled code of the calling VI.

Inlining subVIs is most useful for small subVIs, subVIs within a loop, subVIs with unwired outputs, or subVIs you call only once. To inline a subVI, place a checkmark in the **Inline subVI into calling VIs** checkbox on the Execution page of the **VI Properties** dialog box.

As with turning subVIs into subroutines, inlining subVIs also has some tradeoffs. A subVI you inline cannot contain recursion, and all calling VIs of the subVI must be static. Also, when you inline a subVI, LabVIEW ignores any priority, reentrancy, or preferred execution settings.

## CVT
Current Value Table: a set of VIs used to store and retrieve data asynchronously from different parts of an application. Based on and similar to the concept of a functional global variable 
#### Reference
https://forums.ni.com/t5/Reference-Design-Content/LabVIEW-Current-Value-Table-CVT-Library/ta-p/3514251

![[notes/software/labview/images/CVTUses.png]]

## FGV
Functional Global Variable

