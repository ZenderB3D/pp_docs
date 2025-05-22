#Quick Rig - Edit Armature:  
  
As the name suggest, it's a tool that lets you edit armatures. More precisely, this is a modal operator that wraps around actions you might make when you take an armature to edit mode.  
  
What this means is that pistonpusher can detect changes and do something based on them. It can do a variety of things:  
  
* Smart adjust - Translate vertices and objects based on the difference in bone length if bones changed. This behaviour can be disabled per bone, alternatively, you can configure 'center' points, also on a per bone basis  
* Bone 2 mesh - Add cylinder or cube primitives based on bone length  
* Joint 2 mesh - Add cylinder or cube primitives at bone tail/heads  
* Toggle bone display type  
* Toggle bone axes  
* Undo all - Undo any changes/set to rest pose  
* Temporarily detach any children. Including relations made with a child of constraint and bones that target your armature with child of constraints  
* Automatically unparent orphaned objects(if parent bone was deleted/not found)  
  
  
#Smart adjust:  
  
This system will adjust objects that are immediate children of any bones that changed during an edit mode session. For tail ends this is done automatically by blender but with this system, it's also done for head ends. This means that origins are preserved if they are at a bone head/tail location.  
  
Center/half points are based on the state of any parent bones when the operator was started, as this state aligns with the state of any child objects until you exit edit mode. The circle that appears when you changed a bone (having children) indicates the exact point where a mesh will be halved.  
  
Objects that use child of constraints are also supported but these are treated differently: These will never have their mesh stretched(even if mesh object), which side they adjust to is based on distance to parent bone tail or head.  

#Bone 2 Mesh / Joint 2 Mesh  
  
Spawns primitive objects, a cube or a cylinder at the location of bones or tail/head ends. Joint 2 mesh results in rotated primitives and you can define a primary axis that controls this rotation.  
  
Bone 2 mesh will scale/stretch the object to match bone length.  
  
Joint 2 mesh will target whichever linked bone is the child bone, it also works on unconnected tail or heads.   
  
#limitations:  
* Can't rename existing bones while this operator is active, only NEW bones  
* Smart adjust stretching only works with mesh objects currently  
* Tool expects an armature at rest-pose. Note that constraints including IK may affect a chain and technically pose it as well. Testing proved that to a certain degree it will work with minimally posed armatures  