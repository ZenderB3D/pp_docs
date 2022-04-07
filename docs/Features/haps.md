#Hose Attachment Points  

Hose attachment Points are a geometry node solutions to creating extrusions onto curved surfaces without having to alter/clean up geometry. Together with the Set up HAP data transfer operator, it's one of the fastest way to achieve this. It can set up vertex groups and data transfers for pretty much perfect normals.*  
  
>*Visually they are pretty much perfect but a sharp observer might notice minute differences when compared to the real deal. I doubt most people will notice this initially. These are very small differences related to how one can mix the normals of the two objects. So it's partly a matter of preference/taste as well. At typical viewing angles and distances these can absolutely be ignored. 
  
The geometry node modifier of a hap placer simply spawns instances for every vertex it finds. 
  
This video explains the core usage basics:  

<iframe width="560" height="315" src="https://www.youtube.com/embed/aY-qu_xp5Es" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 
  
How to use it with existing piston instances/parented objects(v4.0.2+):  
  
<iframe width="560" height="315" src="https://www.youtube.com/embed/xvUeWWZ6yWM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  

*Limitations/Drawbacks*  
* Data transfers will be resource intensive, even more so on objects that are hooked. Disabling viewport visibility of the data transfer modifier, or applying them are two ways to get around that.  
* While workable at smaller scales, it prefers a rather big scale to work with. This has more to do with floating point imprecision. In the future I will explore optimizations. For now, reducing rim bevel segments should give the data transfer operator enough error margin at smaller scales.



 


