#Piston snap modal/tool

There are both a snap tool and modal. The tool provides numerical input and uses the targets differently than the modal operator. For most usecases the snap modal is probably the better choice. You can choose which one you want to use in the add-on preferences. It's set to modal by default.

**The piston snap modal**

<iframe width="560" height="315" src="https://www.youtube.com/embed/NRG7CG37kPU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

>Note, you can also re-snap a piston that was already constrained. If you have two empties selected and make a selection in the pop up menu, you will append/instantiate and start the snap modal.

>The target empties have to be aligned along their local Y axes.

>It also 'restores' a piston to its default set up, so that the B empty is a child of the armature again before it gets snapped. 

>To get your target empties, simply snap one empty into place, like a mount, rotate it so that the empty's Y/-Y axis points in the right direction, like that of another mount, then duplicate and move along local axes. You can use the track to and apply operator for this.

>**hotkeys:**  
>S - toggle scaling  
>R - rotate by 45 degrees along local Y  
>E - toggle length anchor position  
>c - constrain on finish  
>LEFT arrow - cycle piston type  
>RIGHT arrow - cycle sub directories  
>mousewheel up/down - toggle direction  
>SHIFT - sensitivity modifier

>Numpad keys allow camera control but certain features won't work in ortho view. 




**The piston snap tool**  
<iframe width="560" height="315" src="https://www.youtube.com/embed/zZwrF0bdsKo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

>The piston snap tool can be used to place a piston quickly, you only need to select a piston armature and two objects. It can also be used directly as you append/instantiate a piston but the re-do panel will not work in this case. 