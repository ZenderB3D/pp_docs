# Simple Bones 
  
Simple Bones is a tool that can be used to create bones based on objects. When done/confirmed, a new armature is created based on the bone widgets and bridges set up. The tool can also append to existing armatures.    
  
Its mostly useful in situations that involve other software like plasticity. I often export simple planes to capture origins and/or rotations. I do so because, unless carefully exported and/or remeshed, geometry isn't always reliable for capturing centers/origins.
  
In short, this tool can capture these origins and place bones in a logical manner, based on the axes of the origin plane/reference object used. 
  
Objects qualify as an 'origin plane', for this tool, if: 
 1. Object is of type 'MESH'  
 2. matrix_world is identity (0,0,0 location and rotation, 1, 1, 1 scale)  
 3. Object has exactly 1 face 
  
The operator will rely on object transformations/matrices should any of these conditions be false. (eg. Empties)  
  
Placing bones is done with 'Bone Widgets'. By themselves, bone widgets are mainly ideal for control/secondary bones, or, bones that don't require a specific length.  
  
For bones that have to be of a specific length, there are 'Bridges', which combine the data of two bone widgets. 
  
Both types of interfaces will roll the resulting bones, indicated by their grids when selected/active.  
  
Should your bridges connect such that they form bone chains, holding CTRL and pressing LMB/RMB will either add or remove a relation to the highlighted chain.  
  
<iframe width="560" height="315" src="https://www.youtube.com/embed/eDz-pBrr9aA?si=2QB6yR1-AGGNLTfa" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>