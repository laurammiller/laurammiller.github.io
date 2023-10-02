---
title: LabVIEW Style Notes
feed: show
date: 2023-09-28
tags:
---
Reasons to care about style:
- helps other programmers understand your code more quickly
- helps "you" understand your own code in X months when you come back to it
- helps with debugging
- makes it easier to add changes or features later
- helps you stay consistent
Linked to [[notes/software/labview/LVTips|LVTips]]
## Icons

### Background 

- LabVIEW icons are layered.
- Merging layers down to the NI icon layer can cause issues later when a class banner or icon is updated
- For class icons, the layers are ordered with the class icon behind the class banner
### bugs/issues
-  if the border of the labview icon is too light, the text will smoosh

## Wiring

- No wire bends
- choose a bus or a priority class that is always wired in the straight line
- "snap" the wires
- clean up any coercion dots

## Error Handling
- consider not wiring the error wire for simple accessors where it isn't being operated on
- Automatic Error Handling - be wary of leaving this on.

## Connector Pane
- Default connector pane to required

## Block Diagram
- Add a light grey background to alternating structures on the block diagram to make the structures visually easier to distinguish