---
layout: post
title:  "A5 pt. 1: Getting Meshy"
date:   2022-11-7 8:53:52 -0700
categories: Assignments
---

Meshes are not my friend. At least, not merging meshes that other people have created. 

## Merged Meshes

Here are my final merged meshes. They are all closed meshes that rhino reports as being "a good mesh" 

![Rhino screenshot of teardrop mesh](/Digital-Fabrication/assets/images/A5-1.png)

![Rhino screenshot of three merged mesh vases](/Digital-Fabrication/assets/images/A5-2.png)

![Rhino screenshot of mesh analysis](/Digital-Fabrication/assets/images/A5-3.png)

My concept was to create a vase with a solid part and a patterned/texture part. I really thought that this was going to be easy and quick, but I was very wront about that. I did learn a lot about meshes along the way! 

## Process (and Failure)

My process had a lot of this...

![Rhino screenshot of a bad boolean result](/Digital-Fabrication/assets/images/A5-4.png)

And this...

![Rhino screenshot of a bad boolean result](/Digital-Fabrication/assets/images/A5-7.png)

And this...

![Rhino screenshot of a bad boolean result](/Digital-Fabrication/assets/images/A5-8.png)

I started with two droplet vases. One that was solid, and another that had a lattice design. My plan was to use a planar surface to boolean split the vases at an angle and then use a boolean union to join the two halves of the split vases to make one closed mesh. It took a lot of troubleshooting to get that to work. 

I worked with three different meshes to make my final merged designs. 
1. Droplet vase
2. Lattice vase
3. Squiggles vase

The meshes I was working from more complicated than they seemend. 

The lattice mesh was actually 52 seperate meshes overlapping each other. Having so many intersecting facets creates complete chaos when trying to do boolean operations. After hours spent trying different methods to split, merge, and repair all these meshes together I decided to give up on the lattice vase and try using a different model instead. 

The squggles vase was surprisingly well made for its complexity. It was a single closed mesh that had a good mesh report. This made working with it easier. 

The Droplet vase seemed like it was a good mesh. It also was a single closed mesh with a good mesh report in rhino. However, only at the end of my process did I check the vase in Cura and find that it it actually has an issue at its base. This issue is present in all of my models that use the base of the droplet vase. 

![Cura screenshot of mesh error](/Digital-Fabrication/assets/images/A5-9.png)

I spent about 4 hours trying different methods for creating a merged mesh from the lattice and droplet vases. I hit a wall and decided that the best thing to do would be to try over with a different mesh. Sometimes starting over really is the best path. I went back to Thingiverse and found the squiggles vase (called the pill vase on Thingiverse, but I think squiggles is a better name). I went about the same process using the new mesh and it worked much better. It really was as simple as splitting using boolean split, scaling so the two mesh faces were about the same size, and using a boolean union to merge them together. Since I finally had success making a few combined meshes, I decided to go back to the lattice vase and try that one more time. The best I was able to do was create a union between the base of the teardrop vase and the solid interior of the lattice vase. Each intersecting line is still an individual mesh which makes it a bad mesh overall. 

I did learn a lot about meshes, and mesh operations by going through this process. Here are some of the my main takeaways: 

1. Start with a good mesh if you can 
2. Check the starting mesh in whatever tool you might use for digital fabrication (e.g., Cura) before starting to work with the mesh. Cura uncovered issues that the rhino report did not have. 
3. Reducing meshes holds hidden magic 
4. Don't use rhino commands like blunt objects. Take the time to actually think through what you are trying to do, and why something isn't working. How is the program thinking? 
5. If you can, just don't use someone else's mesh... 

I probably spent too much time working on my meshes, and not enough time working on my lamp. But, I think that what I learned here will help me with modeling in the future. 


## Assets
**The only printable mesh**

[Mesh Cup](/Digital-Fabrication/assets/files/Mesh-2A.stl)

**Other Meshes**

These are "a good mesh" and a "closed mesh" according to Rhino, but prompt a model error in Cura. This was something that was an issue with the original model I was working from. I didn't realize that until my final check at the end and at that point it was time to move on to the next part of this week's assignment, lamps! 

[Teardrop Vase Mesh](/Digital-Fabrication/assets/files/Teardrop%20merged%20mesh.stl)

[Aligned solid to squiggles vase](/Digital-Fabrication/assets/files/Mesh-2C.stl)

[Offset solid to squiggles vase](/Digital-Fabrication/assets/files/Mesh-2B.stl)

**Source files**

[Droplet Vase on Thingiverse](https://www.thingiverse.com/thing:30889)

[Lattice Vase on Thingiverse](https://www.thingiverse.com/thing:1359035)

[Pill Vase on Thingiverse](https://www.thingiverse.com/thing:2966470)

## Lamps! 

This week also included getting a start on our lamps. Find that work on the [lamps page](https://nantig.github.io/Digital-Fabrication//assignments/2022/11/07/A5-lamps.html).


