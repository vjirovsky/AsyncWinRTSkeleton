Skeleton WinRT apps with async page navigation 
====================

Overview
--------------

Default skeleton WinRT apps counts with no asynchronous calls in LoadState method. When LoadState is not market as async, this function is not able to wait for another async call. 
These methods (LoadState, SaveState) cannot be easily marked as async, because of LayoutAwarePage module. 

These solutions contain modified LayoutAwarePage module with support of async call for LoadState and SaveState methods.

- In **GridApp** folder is full Visual Studio (2012) solution package of Windows Store Grid App template with this modified file and added examples how to use it.

How to use it in your project?
--------------
- Copy Common/LayoutAwarePage.cs to your project and **fix namespace of this file**!  
- Modify state function declarations on every page in project
- *That's all* 


