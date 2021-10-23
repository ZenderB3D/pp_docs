# Adding your own parts and templates

Yes you can!

**Parts**  
Adding parts is quite easy and best demonstrated with gifs:

Mounts(and connectors):  
![Mounts and connectors](../gifs/makemountcon.gif)

> Child objects are supported. The biggest/main object however, should be the active object. Take note of the origin of the main object. Even if the mount pivots at a different location, this origin should be at the world origin(x, y axes). Origins do not matter much for connectors.

Rods:  
![Rods](../gifs/makerod.gif)

>If the rod comes with multiple child objects, you only select 1 child object and lastly the rod. **For rods the scene should be empty and only contain to-be rod objects to make this work properly!**


**Templates**  
At the bottom of the documentation page on blendermarket there is a reference sheet describing what's required/possible. I tried to keep it as simple as possible! Most of what you see in a template is completely optional. I use drivers that derive input from an empty its location for some templates.