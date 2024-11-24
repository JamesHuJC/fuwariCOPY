---
title: "Call In Editor" doesn't get ran - Script Guard Usage Guide
published: 2024-11-24
description: ''
image: ''
tags: [UE5, cpp]
category: 'UE5'
draft: false 
lang: ''
---
## Problem
Sometimes, when you have a "Call In Editor" function/event, and you call it in editor, some of it's cpp code doesn't get run.  
For example:
```cpp
//A delegate you made
DECLARE_DYNAMIC_DELEGATE_OneParam(FDelegateFoo,int,Result);

//Initialize callback
FDelegateFoo Callback=Something;

//Use callback
UE_LOG(LogTemp, Warning, TEXT("Debug!"));
Callback.ExecuteIfBound(123);
```
The text "Debug!" is printed, but the callback isn't called.

## Cause
For some reason, ue5 doesn't run certain functions while in editor mode. 
## Solution
Adding a ScriptGuard will make sure the functions get ran:
```cpp
FEditorScriptExecutionGuard ScriptGuard;
Callback.ExecuteIfBound(Result);// Is ran!
```