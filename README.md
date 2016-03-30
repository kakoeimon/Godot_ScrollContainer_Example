# Godot_ScrollContainer_Example
A simple example of the scrollContainer of Godot.

From my answer in the forums.

You add a Node Scrollcontainer, then add a Child Node ( VBoxContainer for vertical or HBoxContainer for horizontal listing) to the ScrollContainer. 
Set the Separation of the VBoxContainer (or HBoxContainer) to the value (in pixels) you want the objects to be Separated.
After that you can add child nodes to the V(H)BoxContainer and you are done.
NOTE1 that for the child notes to be listed those nodes must be Control nodes. For example if you want to have a scrolling list of Buttons the Child Node must look like this :
Control->Button.
The reason is, if I understand it correctly, that the V(H)BoxContainer will automatically change the position of the Control nodes to fit the Separation value.
Note2 The last child of the V(H)Boxcontainer may not be listed, for reasons unknown to me, the easy way to bypass this is to add a Control node as the last Child Node.
