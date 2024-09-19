---
title: Random Blueprint Tips
published: 2024-07-01
description: ''
image: ''
tags: [UE5, Blueprints]
category: UE5
draft: false 
---
### add " " to variable names
If your variable is named "apple", and somehow you need another thing that also is called apple. You can name it "apple ", note the "space" at the end of apple.  
A usecase for this is: you want to convert a macro into a function. The macro is named "foo". Naming a function "foo" will not be possible, but naming it "foo " will. I know this can cause ambiguity but it is a trick nonetheless.  
Sometimes you can name a function input " " to make it seem cleaner/you can't think of a good name.
### Way to select event/function.
Select the event/function node in bp, press f2(or whatever your rename key is), and you've successfully selected the event/function. This is rarely useful but sometimes it is.
### Right Click Scroll
You can hold right click on use your mouse to scroll in a lot of places. e.g. functions list, output log. This is a bit faster than normal scrolling (for me at least.)
