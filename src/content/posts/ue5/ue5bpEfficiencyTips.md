---
title: Unreal 5 blueprints Efficiency Tips
published: 2024-06-11
description: ''
image: ''
tags: [ue5, efficiency,tips]
category: ue5
draft: false 
---
## Efficiency
### Better Keybinds
You can change keybind so they are easier to reach, for example:
| Function | Old Key | New Key |
| ----------- | ----------- | ----------- |
| Delete/Remove | Backspace/Delete | x/Backspace |

Delete requires your right hand, you have to take your hand off your mouse to press it, but x can be pressed with your left hand.

### Plugins
#### **[Blueprint assist](https://www.unrealengine.com/marketplace/en-US/product/blueprint-assist)**   $20  
Formats blueprint nodes for you. Can't live without this plugin.  
Note: There are other formating plugins, though I haven't tried them. So I can't be sure of their quality.


#### **[Spawn Node Extension](https://www.unrealengine.com/marketplace/en-US/product/spawn-nodes-extension)**   $5  
In ue5, you can hold "b" and press left click in a blueprint to create a branch node, this plugin expands on this feature. You can setup custom nodes such as "not","print" 
![image](<Spawn Nodes Extension.png>)
My settings:
| Key | node | class path |
| ----------- | ----------- | ----------- |
| W | while loop | /Engine/EditorBlueprintResources/StandardMacros.StandardMacros:WhileLoop |
| E | equal | /Script/GameplayTags.BlueprintGameplayTagLibrary.EqualEqual_GameplayTagContainer |
| Q | print | I'm using a custom plugin for printing |
| G | get | /Script/BlueprintGraph.K2Node_GetArrayItem |


### **Many videos about plugins on yotuube**
There are many videos about plugins on Youtube, I recommend giving them a watch. Besides plugins, the tips and tricks videos are also good.  
