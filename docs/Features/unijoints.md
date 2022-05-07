#Universal (cardan) joints

Pistonpusher offers a simple universal joint rig. It comes with placeholder objects which can be changed as you see fit. So long you don't change bone names or remove any, the combine joint operator can be used to combine this joint with a piston. This will also rename the objects and make the cardan joint collection a child of the piston instance collection.  
  
To combine a universal joint with a piston, select the universal joint armature and then the piston cylinder, piston rod or another object that can be tracked and click on the 'combine joint' button in the tools section. If succesful, a 'JOINT IS SET UP' message will appear. Theoretically this should work regardless of orientation but I recommend doing this before a piston is placed or moved.  
  
This action will re-parent the respective original piston anchor to the universal joint rig, which will then act as the new anchor for that side. The snap modal does not support pistons with universal joints. Disable the 'reset new instances' opt-in if you need more instances.  
  
Lastly, the universal joint rig has 3 bones that are relevant for users. The a, b and c bone. a and b represent the mounting pieces, c is the cross object. Objects should be a child of these bones only. B should always point towards the piston. 



