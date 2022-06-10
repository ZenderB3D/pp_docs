# Cable/Hose rigs 

This operator can rig a selection of 1-3 objects. The active object should always be a curve, if not, the operator won't be visible. Transforms do not need to be applied. Can set up itasc solver 3 point control rigs as well.  

To create an IK chain that can be used right away, additional objects have to be selected as well. The origins of these objects, in combination with the curve, are used to create the control bones:  

![preferences](../images/qrhc1.jpg)  

![preferences](../images/qrhc2.jpg)  

- Curve resolution can be changed beforehand but unless the curve is really long, the default curve resolution of 12 should suffice. A better strategy would be to use a subd modifier to later on if needed.  
- Curve bevel resolution is set to 6 but only if it was higher than 6 to prevent (performance) issues due to geometry density.  