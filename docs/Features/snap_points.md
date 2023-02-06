# Snap Points  
  
Snap points are essentially just locations and rotations, or matrices, or something akin to empties. They are owned by and stored on objects as matrices in a custom property.  
  
To add, remove and otherwise manage them, there's a manager (modal operator) which you can access by pressing mouse button 5 or whichever key you bound it to in add-on preferences. The manager closes on key release but this can be prevented by tapping the space bar key.  
  
With the manager running/open, you can add and remove snap points, set focus objects or mirror snap points if their owner has a mirror modifier. A snap point can be exposed as an actual empty or through the 3d cursor by pressing 1 or 2.  
  
Other tools can access the snap points manager python class responsible for all the leg work, currently, the snap and drag tool and the piston planner tool can access snap points by pressing the TAB key to toggle them on/off.  
  
Other add-ons can theoretically access the above mentioned python class as well and access the system in exactly the same manner as I can, which may be interesting in the future.  
  

# UI  
  
* White circle will snap to the snap point 'closest to mouse'  
* Isolated objects receive a yellow circle around their origin, if objects are isolated, only snap points belonging to those objects are shown  
* Operators can allow you to mark a snap point if a selection of multiple snap points is needed. Marked snap points receive an orange circle  
* Yellow dotted/striped line indicating the owner and distance to owner  
* Snap points of the active object, if any, appear thicker than those belonging to other objects  
    
# Limitations  
  
* Applying transformations on an object that has snap points can result in misplaced snap points  
* In a similar manner, editing its mesh may invalidate a snap point as well  
* Snap points created with the snap points manager mirror option can not be mirrored again  