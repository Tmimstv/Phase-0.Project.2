# Phase-0.Project.2
The first completed project in my 3 year plan to understand systems on a deeper level.

Doing the projects in a different order than originally planned. 

Objective: Create a program with a UAF bug and an out-of-bounds bug

This is project 2, a small memlab to demo UAF and Stack overflow, this exploring stack vs heap.

What/How it demonstrates
Heap
UAF(use after free is dangerous because it attempts to access a space that was already returned)
Pointers should be set to NULL if they’re not in use
Stack
Stack overflow can cause a program to crash
Easiest way to replicate this was to create an array and then have the program attempt to reach past the array.
Arrays have items who are grouped together in memory, so asking it to go to the next memory space after the end is sure to cause problems

Additional Notes:
So we used -fsanitize=address and I’m not gonna lie… I have no idea what I’m looking at. I can see the memory but I’m not sure what I’m supposed to do about it. I do understand though that its pointing out where things went wrong in memory.
-Wall -Wextra & -Werror will definitely save me from a lot of headache in the future.

Currently, I know I don’t fully understand BUT it doesn’t mean I can’t understand.

<img width="985" height="761" alt="image" src="https://github.com/user-attachments/assets/130071fb-f2df-4874-bd98-042e6ffd2d53" />
