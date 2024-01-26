Visual score notes
==================

## 24-Jan

I've created a workflow to create custom icons (or can take from anything else..) that can be rendered in OpenGL space in Jitter. 

So far my workflow is:

- Create geometric shapes in Adobe Illustrator. 
  - Combine paths into one compound path. 
  - Expand > Outline stroke to about 12px (should probably change to different units?)
  - Export as SVG. 
- Convert to 3D Objects in Blender
  - Import SVG
  - Apply material color
  - in Properties > Curve: 
    - Extrude (0.025 measurement now)
    - Bevel (0.03cm, resolution 16)
  - Export as .obj file.
    - I also tried Collada (.dae) but the jit auto_handle in Max are comically too big. Don't know why. 
  - Display in Max
    - jit.gl.model:
      - 'read' file
      - attributes: 
        - lighting_enable
        - smooth_shading
      - position, rotatexyz, etc. for display. 

> Alternate way to render the 2D icons:
> - In Illustrator, export the compound path as SVG
> - In Blender, add bevel till it becomes round. The problem is it does't close the ends of segments, so they look like of shit. Maybe there's a happy medium. 

So, to add this to the main piece, it needs to receive input from Dicy2 output, then display the correct icons. No problem. 
  