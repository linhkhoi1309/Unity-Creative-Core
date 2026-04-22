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

## Shaders

- a script that applies the properties contained in a material to render the meshes of your 3D objects to the 2D image on your screen. 
- each shader is written for a specific render pipeline.

### Types of shaders
- Based on purposes:
    - Fragment shading, also known as pixel shading, is the shading that represents mesh surfaces to produce the color of each pixel in the 2D image.
    - Vertex shading operates on the vertices of the mesh, typically changing their locations to make the surface move or transform. 

- Based on light reflection:
    - Lit shaders respond to the light in the scene, and unlit shaders don’t. 
    - Unlit shaders are useful for certain artistic effects or for optimised projects that run more efficiently by not using lighting.

#### Universal Render Pipeline Shaders
- 2D > Sprite-Lit-Default, Sprite-Mask, Sprite-Unlit-Default: Designed for 2D projects, these shaders are for flat objects only and will render any 3D object as 2D.
- Particles > Lit, Simple Lit, and Unlit: are for visual effects (VFX). 
- Terrain > Lit: optimized for use with the Terrain tools in Unity. As a lit shader, it will render based on the light in the scene that reaches the object.
- Baked Lit: automatically applied to lightmaps.
- Complex Lit, Lit, and Simple Lit: These are all variations on a general-purpose, physically based lit shader.
- Unlit: a shader that does not use light.

## Relationship between shaders and materials

- Shaders can be very specific or quite versatile. 
- A shader can set the color of GameObjects or it can allow color to be configurable by materials. In fact, one shader can make many objects look like entirely different substances, while still giving a scene a unified look.
- Shaders and materials work together as a team — the shader defines what a surface **can** look like, while the material defines what it **does** look like.

## Side notes:
- When a material has a shader that is mismatched to the current render pipeline, it is bright magenta (pink) to alert you.