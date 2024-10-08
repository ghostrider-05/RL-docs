---
title: CSG
---

# Constructive Solid Geometry

![Two maps: one with default textures and one with custom textures](/images/udk/basics/comparison_textures.png "You vs the map she tells you not to worry about")

The simplest and most straightforward way to build a map is using UDK’s brush system, CSG (Constructive Solid Geometry). In the days of yore, this was basically the only way people were making maps, until people started using 3D modeling software and following the steps laid out in the first version of this guide in late 2016.

CSG is a great tool for sketching out an idea, but it’s roughly the equivalent of using Paint for your big school presentation instead of PowerPoint. I believe that with a truly minimal time investment learning Blender or another 3D modeling program, you will fly past the capabilities of CSG brushes in no time.

However, if you must, here’s how you can use CSG brushes.

## The CSG Toolbars

![Brushes buttons in the UDK menu](/images/udk/essential/ui_editor_brushes.png)

---
![CSG buttons in the UDK menu](/images/udk/essential/ui_editor_csg.png)

- Top Left: Add (Ctrl+A)
- Top Right: Subtract (Ctrl+S)
- Bottom Left: Intersect (Ctrl+I)
- Bottom Right: Deintersect (Ctrl+D)

If it is not already visible, **press `B` to reveal the CSG brush.** It has a dark red outline, and a red square will appear on each corner when you select it. To change its geometry, select a different option in the Brushes panel. If you want an exact size or to change parameters of a brush, right click the button and enter your values.

You can move, rotate, and scale the brush just like anything else in the scene. Additionally, you may add special volume types with the Volumes panel. These volumes may be revealed or hidden with `O`. **You will have to add a BlockingVolume after every CSG step if you wish to collide with your creation. However, rectangular collisions will almost never work as expected.**

One workflow option is to select a face of your CSG object, press Shift+S > File > Export OBJ. You could then clean up this mesh in Blender and re-import it.
