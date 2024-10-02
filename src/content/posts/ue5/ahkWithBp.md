---
title: ahkWithBp
published: 2024-10-02
description: ''
image: ''
tags: [ue5,Efficiency,ahk,Blueprints]
category: 'ue5'
draft: false 
---
AHK(auto hotkey) let's you script your custom hotkeys. Certain hotkeys can be useful for ue5.  
For example:  
```
#SingleInstance Force 
^e::Enter
^d::BackSpace
return
```  
This script maps "ctrl e" to "Enter", and "ctrl d" to "Backspace". Hitting "Enter" and "Backspace" requires your right hand (normally), but your right hand is on your mouse making blueprints, only your left hand is on the keyboard, this is where the hotkeys come into play. Similar techniques can be found in my "Creating Blueprint Nodes With One Hand" blog post.  

(more hotkeys might be updated later)