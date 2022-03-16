# Lab 5  
I found the tests by searching through manually.  
## Test 512:
```
[link] bar](/uri)
```
Given Output: `[/uri]`  
My Output: An infinite loop.  
The Given implementation is correct because the expected output is `[uri]`.  
While working on another part of my implementation, I had commented out the code block that handles nested brackets. I can fix this bug by undoing the //.  
## Test 516
```
[![moon](moon.jpg)](/uri)
```
Given Output: `[moon.jpg]`  
My Output: `[/uri]`  
My implementation is correct because the expected output is `[/uri]`.  
The bug in the Given implementation could be fixed by checking for an exclamation point immediatly before an open bracket, to determine if it is a link or an image.