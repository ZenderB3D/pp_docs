#Installation

You can install pistonpusher like most other add-ons. Open blender, go to preferences, click on addons, click on 'install...' and select the pistonpusherxxx.zip where you downloaded it. Don't forget to activate it.

Assuming you downloaded the pistons and piston parts zips, you should extract these at a location of choice. Once done, navigate to the pistonpusher add-on preferences in blender. You'll have to point the add-on to these directories. It's recommended that you use blender's filebrowser for this as the string should contain a trailing backslash (on windows, this is os dependent)

There is also a kpack, see kitops manual on how to install it if you haven't done it before. It's a very similar process.

#Updating

If replacing the files fails:

First remove the add-on in blender and then restart the client. Now you should be able to re-install the add-on safely.


#General usage

If you hid the n-panel, all features are accessible from the pistonpusher pop up menu. The default shortcut is **SHIFT+E**.  

To append/instantiate a piston, you simply select a thumbnail. New instances are always 'reset' to a sort of default expected state. This means that the B empty will always be re-parented to its host armature even if the last instance was already placed and constrained.  

Depending on object selection, a piston will be placed at an object's location, the 3d cursor or the snap tool/modal will be started. 

