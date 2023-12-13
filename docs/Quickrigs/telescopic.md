#Telescopic Pistons 
    
You can easily add more rods and later remove them, to/from any pistonpusher piston by selecting the rod and any piston object. Then open the quick rig menu and the options should be available. To remove them, select any piston object, open the quick rig menu and choose 'remove rod'. This will start removing rods, starting with the last one added.   
  
These rods should be simple cylinders during set up, with their origin at whichever end is closest to the B empty. Once set-up, you can add detailing objects and parent them to their respective rod bones.  
  
The operator briefly shows an abstract representation of the extended piston. If an ERROR icon appears in the re-do panel, you should specify the original rod or add an object that will qualify as it. (object should not be more than twice as short as longest rod found and be a child of the piston rod end bone for the operator to recognize it)  
  
The behavior/results achieved by changing the leading or trailing distance settings per rod depend on FIFO mode. In a nutshell, when FIFO mode is ENABLED, trailing distance works similar as leading distance when fifo mode is DISABLED but in reverse. Leading distance while FIFO mode is ENABLED lets you override the FIFO order for that specific rod only.  