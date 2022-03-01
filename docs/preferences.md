#Add-on preferences


![preferences](../images/preferences.jpg)  

#Main settings
**Assets directory** - A path pointing to your assets directory. It does not need to be set anymore but it's recommended to prevent data-loss during updates.  

**Updating** - A button may appear prompting you to update your library, note that it may appear even if no new parts have been added. Please refer to the changelog as i'll always mention new additions!  
  
> It is also possible to remove and create version files to trigger updates or get rid of the warning/button if you know the library does not need an update.  
  
  
#Asset Management(import/export/merging directories)
A tool was created to handle file indexes. It can handle both piston and part directories. It's agnostic as far as the files and their intended purpose goes. This means the user has some responsibility and it should be used with care. The tool can not execute if the source path is in the currently used library. It only updates indexes of the source files so that they match after copying. I recommend never using it on another library if that library will be used by pistonpusher at a later time!  

Sharing your works, for whatever purpose, is as simple as making a .zip/7z archive of your specific user parts directory(or simply the whole user directory). The recipient can then merge them as required. If no user parts are present(recipient) you can just move the files, assuming their indexes have not been touched by this tool.  

Importing piston directories was already just a matter of copying/cutting a directory, now you can also merge into existing directories. Just beware that it does not check for duplicates of any kind.  

It tries to catch simple mistakes based on parent directories but this may not always be accurate, if you wish to ensure this is accurate:

The structure of your files, at the very least, should look like this  
  
>'Pistons' directory  
>	'Your pistons subdir(s)'  
  		
or  
  
>'Piston parts' directory  
>	'Your user parts' subdir  
>	(optional)'User' directory  
>	    (optional)'your user parts' subdir(s)  
  
If an incompatible match up is detected, a warning will appear and the 'Merge directories' button will be disabled.  

If executed succesfully, paths will be cleared and some information is printed to the console.  
  

  
#UI
**Create in n panel only** - Removed as of v3.4.4

**Hide n panel** - Removed as of v3.4.4

**Notification duration** - The length that a notification stays visible.(Fade out including)

**Notification location** - Change the location of notifications. It's recommended that you only change the Y axis value.

**Notification (text) size** - Change the size of notifications.

**Warnings location** - Change the location of custom mode create onscreen warnings.  

**Warnings (text) size** - Warnings size. This value also decides the text size of other onscreen ui elements like that of the set bone as parent tool.  

**Center plane size** - Change the size of the (custom) center plane that's visible when the armature solver overlay is enabled.


#Advanced
**Collection to append** - This is the piston (o)riginal collection. You can change this if you prefer so.  

**Custom plural** - This value affects how 'type' collections are named.  

**Custom singular** - This value affects how 'instance' collections are named.  