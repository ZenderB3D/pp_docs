#Parent Wizard  
  
The parent wizard is a bi-directional parent-child relation manager tool. It offers a color based interface, highlighting geometry. The hud also has a fall back 2d mode for objects without mesh data or armatures and their bones. Additionally, objects with high poly meshes use the 2d hud as well(performance reasons).
  
Where possible you can control the type of relation you're setting, if required, the tool overrides your input. This however mainly concerns removing relations and pose bones.  
  
You control the tool mainly with the left and right mouse button. LMB acts as a sort of shift select, adding objects to your selection. If you select in empty space, your selection is cleared (Except for any selected pose bones). Once you selected an object, you can hold SHIFT or CTRL and then select another object. This will pre-select the object and add or remove a relationship. This is also indicated by the green and orange color (respectively). Armatures and their bones can be accessed by hovering the mouse over an object and then pressing space.  
  
  
#Colors  
* Red: Parents  
* Blue: Children  
* Green: Add relation  
* Orange: Remove relation  
  
#Keymap
* LMB: Select object, confirm relation  
* LMB + SHIFT or CTRL: Set relation target/pre-select  
* RMB: Cancel relation, Exit/finish operator  
* Mwhl + CTRL: Scroll visible bone layer(Pose mode only)  
* `: Reset bone layer visibility(Pose mode only)    
* H: Hide/Unhide hidden bones(Pose mode only)  
* TAB: Toggle constraint/object level relation
* Q: Toggle Parent/Child relation  
* W: Toggle relative mode  
* B: LMB passthrough, use for box select, lmb or b after selection will process the selection  
* SPACE: Toggle OBJ/POSE mode, hover mouse over armature(bone) and press space to access bones  
* 1: Deselect all, even pose bones  
* ESC: Exit/Finish operator  