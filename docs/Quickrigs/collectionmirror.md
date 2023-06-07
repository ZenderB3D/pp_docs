#Collection Mirror Tool  
  
A tool designed to mirror assemblies of rigs and their attached baggage so to say. It is called the mirror collection tool because it requires a collection active and selected in the outliner.     
  
When this option is selected, additional parameters will appear which you can use to get the result you require.  

Additionally, the behavior of this tool can be influenced to tweak the results if issues arise, this is done by tagging object names:

- _APPLYSR - Use when scale/rotation of an armature should be applied after mirroring it  
- _APPLYS - Use when scale of an armature should be applied after mirroring it  
- _RST - Use when posebone child of constraints must be set to inverse after mirror operation (if the mirror operation failed on a specific armature, go to pose mode, find a child of constraint and hit set inverse, if this fixes it, you should use this tag)  
- _OBLCL - Mirror every child of this armature. May require that rotations are applied  
- _LCL - Use to mirror this object locally  
  
The order of these tags does not matter! The first 3 tags only work on armatures.
