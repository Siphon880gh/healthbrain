
Spin extrude vs Spin Duplicate (with the 3d cursor as pivot point)
[https://blender.stackexchange.com/questions/161454/what-is-the-difference-between-spin-and-spin-duplicates](https://blender.stackexchange.com/questions/161454/what-is-the-difference-between-spin-and-spin-duplicates)

---

**Spin tool (aka spin extrude tool)** 
Extrudes the face of the cube around the 3d cursor pivot point

**Spin with duplicates tool**
Duplicates the face of the cube along the circular path around the 3d cursor pivot point. It's duplicated evenly.


---

## Instructions

How to finalize spin extrude or spin duplicate is at the end

1. Set the 3d Cursor to where you want the pivot point of the circular path to be
2. Select what you’re spinning. Here we select the face of a cube

![](https://i.imgur.com/T0lJnau.png)

2. Choose either spin tool or spin duplicate tool* - doesn’t matter which  
    Choose either. Blender in Q1 2024 has a bug where both tools act the same, and you have to open the operator box (appears right after applying the tool), then either untick or untick "duplicate" for Spin or Spin Duplicate, respectively.

3. Use the radius dragging handler:
![](https://i.imgur.com/pes22JK.png)

4. As discussed above, you now have to tick or untick the duplicate option in the Operator box

Tick “duplicate” if you want to use Spin with duplicates
Untick “duplicate” if you want to use Spin (Extrude)


Spin with duplicates:
![](https://i.imgur.com/bJHXOij.png)

Spin (extrude):
![](https://i.imgur.com/yFGe9U9.png)

While tool is selected, you can lock the spin to an axis or axes at the top left
![](https://i.imgur.com/O9R5ex0.png)

If you lock more than one axis (SHIFT+Click), then two rotation handles will appear allowing you to switch spinning between the two axis