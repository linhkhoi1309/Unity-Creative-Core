# Shaders and Materials

## Meshes
- the 3D skeleton of your GameObject
- every GameObject in Unity has a mesh
- the geometric element of the object.

### Mesh data
- a series of flat 2D polygons defined by vertices (singular: vertex), which are points in 3D space that are stored as XYZ coordinates.
- normals, which are additional values that define the direction the surface is facing. 

### Mesh Filter
- points to the mesh coordinate data in your project. 

### Mesh Renderer
- specify how the mesh will be rendered. 

## Materials
- an asset that works with a shader to define how meshes will be rendered
- one material can be applied to many meshes.