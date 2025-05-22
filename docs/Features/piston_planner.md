#Piston Planner Tool  
  
A tool that can be used to place existing pistons or establish a 'work' plane to model one. In more technical terms, this is a vector/matrix based orientation tool.  
  
##Why  
  
To properly explain why this tool is needed, it's important to understand that *quick rig - simple piston* is called 'simple' because it can only deal with simple geometries. This is based on the following axiom:  
  
*A typical piston/actuator will only travel in at most 2 dimensions*  
  
Which tends to be true for the vast majority, if not all real-life applications of actuators. 3d artists often (over)use ball joint actuators. Please note that in this context, *geometries does not refer to mesh geometry but rather the difference in location between the actuator mounts and 'roll' around the vector/axis formed by these 2 locations.*  
  
So in other words: Almost all actuators that move in 3 dimensions are fixed to another set of mounts/devices specifically designed to facilitate this motion. This also means that, by approaching the situation logically, you'll find that this tool will also work in more advanced setups. Namely, to get started, you'd have to figure out a mounting solution first and from there the rest can follow. Tracking constraints may be used to align the first set of mounts towards each other.  
  
  
##How it works  
  
Once the tool has been started, you can use objects and/or geometry to define locations. First the pivot points. Then a vector representing the side of your actuator, or the amount of roll, this also requires 2-4 locations(2 red vectors for advanced setups). At this point the tool has enough information to form a matrix which is used to orient the empties.  
  
Note: You can also Click and Drag to create vectors. This also works while changing between obj/mesh mode!  
  
This tool, by itself, will only spawn correctly aligned empties. This keeps the tool fairly low level and leaves the rest to the user. If you already have a model in place, set the origins of at least the root objects to their respective side/empty. Otherwise, the empties can be used as a starting point for your model.  
  
#Troubleshooting  
  
'Angle not 90d or zero length vector detected, op reset'  
  
Indicates that 2 locations were in the same location (zero length vector) or that the angle between the green and blue lines/vectors is not 90 degrees, for whatever reason. Usually this hints at a modelling or placement mistake.  
  
  
#keymap:  
* LMB/RMB - Basic tool usage  
* SPACEBAR - Select obj or Toggle obj/mesh mode if possible  
* Q - Get center - Get center between the currently selected location(yellow) and the highlighted one(red)(mesh mode only)  
* W - Use edge - Use edge to define points  
* E - Loop center (Angle based)(Edge), works similar to get center if a location is already selected  
* 1 - Set 3d cursor - Sets the 3d cursor to the first added location on finish  
* Tab - Access snap points  
* 1/2/3 - Use snap point axis to define points  
* ESC - Exit/cancel  
