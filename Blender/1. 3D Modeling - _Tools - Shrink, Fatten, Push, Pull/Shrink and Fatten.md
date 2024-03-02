
It's resizing based on normals of a vertex.

Reworded: This operation adjusts the vertices of a mesh along their normals, either moving them closer together (shrinking) or further apart (fattening). It's particularly useful for adjusting the thickness of an object without altering its overall shape in the way uniform scaling would. For instance, you might use it to thicken a wall or to add volume to a character's limbs. This operation doesn't scale the object in a traditional sense but rather moves the vertices in or out along their normals.

---

How activate: ALT+S instead of S
Or: SHIFT+Space and select Shrink/Flatten

---

To best exemplify this, create a cylinder, go into Edit Mode, then set Selection Mode to Polygon Face

You can see that the polygon face is along the X axis (red):
![](https://i.imgur.com/JlxmyTI.png)


So lets resize along X by pressing: R -> X

![](https://i.imgur.com/8BKqix9.png)

----

Instead of S->X, lets do shrink/flat with ALT+S -> X

In one direction:
![](https://i.imgur.com/W3QcdC1.png)

In the other direction:
![](https://i.imgur.com/71nkxGt.png)

---

Also lets you thicken a cylinder without making it longer (thickening, hence it's called fatten)
![](https://i.imgur.com/ning0BJ.png)

https://youtu.be/DLZrFZegi5U?t=4

---

Proportional editing:
Not -
![](https://i.imgur.com/pekNm9q.png)

With - .![](https://i.imgur.com/GOmUT5q.png)

^ And you adjust with Offset and Proportional Fall Off

---

![](https://i.imgur.com/uSe0TlC.png)

With Proportional Editing ticked on, you can choose to affect only the connected vertexes or also the unconnected vertexes. Eg. Ticking Connected means the proportional editing shrink/flat will only affect the selected vertexes that are connected and will not affect the eyes which are not connected.

https://www.youtube.com/watch?v=DLZrFZegi5U