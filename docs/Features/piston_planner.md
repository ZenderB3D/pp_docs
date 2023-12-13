#Piston Planner Tool  
  
A tool that can be used to place existing pistons or establish a 'work' plane to model one.  

<iframe width="560" height="315" src="https://www.youtube.com/embed/OdY0FhheqQ0?si=2I5A2MYsc_u6sdH1&amp;start=88" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>  
  
A commonly encountered error:  
  
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
