Fatten:
![](https://i.imgur.com/UzNuLoa.png)

Shrink:
![](https://i.imgur.com/BznwzBS.png)

---

Offset:
Scale the offset to give it a more even thickness.
![](https://i.imgur.com/l1wLVsM.png)

In Blender, the Shrink/Fatten tool is used to move vertices along their individual normals. When you use this tool, it can cause the mesh to expand or contract unevenly, especially if the geometry is complex or the angles between faces are varied. There's a phenomenon where vertices that share faces forming a more acute angle obtain a greater offset factor—relates to how the normals are calculated and how the displacement along these normals is executed.

Here are steps to use the Shrink/Fatten tool and adjust the offset to achieve a more even thickness:

1. **Select the Mesh**: In Edit mode, select the mesh or the specific vertices, edges, or faces you want to adjust.
    
2. **Apply Shrink/Fatten**: Press `Alt + S` to activate the Shrink/Fatten tool. As you move your mouse or use the numeric input, the selected elements will move along their normals.
    
3. **Adjust the Offset**: To control the offset's scale and make the thickness more even, you can do a few things:
    
    - **Offset Even (Alt + S then Alt)**: While using the Shrink/Fatten tool, you can press `Alt` to toggle the 'Even Offset' option, which attempts to make the displacement more uniform.
    - **Correct Face Attributes**: This option helps maintain the texture and vertex colors while transforming the mesh. It can be toggled in the operator panel (`F9` after the operation) or in the tool settings.
4. **Thickness Factor**: The factor by which you scale the offset can be adjusted interactively with the mouse or by typing in a value. If you notice that vertices at acute angles are offset too much, reducing the overall factor can help mitigate this, although it will also reduce the offset for all vertices.
    
5. **Other Adjustments**: Depending on your specific needs, you might want to explore other tools in conjunction with Shrink/Fatten, like the 'Smooth Vertex' tool, to even out irregularities after you've applied the transformation.
    
6. **Manual Tweaking**: Sometimes, automated tools can't provide the perfect result due to the complexity of the mesh. In such cases, manual tweaking of vertices might be necessary to achieve the desired evenness.
    

Remember that the results can vary significantly based on the geometry of the model and the distribution of normals. It might require some experimentation with the settings to get the desired result.
