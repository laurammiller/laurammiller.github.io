---
title: "LVTips"
feed: show
date: "2023-04-19"
tags: 
---

A list of interesting LabVIEW shortcuts

## Swap terminals
1. Hold CNTL
2. Hover over terminal and left click

Works for terminals on various primitives:
![](notes/software/labview/images/swap%20terminals.gif)
But also icon terminals:
![](notes/software/labview/images/swapiconterminals.gif)
## Quick Drop Shortcuts

CTRL+W = Wire selected objects together

## Enum & Ring
Easily select an item using the right click menu
![](notes/software/labview/images/enumselect.item.gif)

## Error Handling

- Wiring errors to an empty case structure will actually ignore the error. make sure to always leave a comment if using this method
	- ![[notes/software/labview/images/ignoreerror.png]] 
- Wire the error in to the first input of a merge error cluster, so that the error ordering remains with the first error being reported first
	- ![[notes/software/labview/images/mergeerror.png]]
- Use a rule if possible to move error wires (z-shift) to the back of the diagram