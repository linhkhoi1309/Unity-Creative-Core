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

### Side notes
- When a material has a shader that is mismatched to the current render pipeline, it is bright magenta (pink) to alert you.

## How light behaves

When light comes in contact with any object, it can do one of three things: bounce off of it, which is known as reflection; pass through it, if the object is transparent or translucent; or be absorbed by it.

## Specular and diffuse reflections

- There are two ways that light reflects from an object: there are specular reflections and diffuse reflections.

![Apple Reflections](References/apple_reflection.png)

### Specular reflections

- is the direct reflection that is most visible on shiny objects.  
- On the apple, the specular reflection is white, which indicates that the light source is white.

### Diffuse reflections

- not all the light that reaches the apple bounces off it directly. 
- other light penetrates the surface, and passes through or bounces around the outer layers of the apple. Some of this light is absorbed and some bounces out. 
- the light that escapes is the diffuse reflection.
- determines its visible color. On the apple, the non-red light is absorbed, and the red light is reflected to our eyes.

## Diffuse reflectivity

- In Unity, to represent diffuse reflectivity the URP/Lit Shader calls for a Base Map.
- Other shaders commonly call this property Albedo or Diffuse Map (these terms don’t mean exactly the same thing technically)

### What is albedo?

- describes the measurement of diffuse reflection. 
- typically specified as a regular color, expressed as three values for red, green, and blue (RGB values). 
- RGB values can be translated to values for hue, saturation, and luminosity (brightness). 
- the luminosity of the albedo color corresponds to the amount of diffuse reflection
- the hue and saturation describe the quality of light that escapes from the surface.

### Why is it called a map?

- Maps can be solid colors or they can be specified with 2D images to add variation to a surface. 

## Metals in the Specular workflow

- The property of a surface that makes it look like metal is called **specularity**.
- Specularity is different from smoothness. We could polish a red apple until it is very smooth, but it would never turn into metal that way. 
- However, to have any specular reflection, a smooth object must have some specularity

- Like diffuse surfaces, metals do absorb light. You can tell this is true if you leave a metal object in the sun — it gets hot! 
- But on colored metals, like gold and copper, the colored light we see is actually not a diffuse reflection — it is a tinted specular reflection. It must be specular because you can see the light sources in that reflection. The tint that you see is caused by the object absorbing part of the visible spectrum of light and only reflecting the tint color.

### Specular workflow

- In the Specular workflow:
    - A shiny metal has a high Specularity setting and a high Smoothness setting.
    - A shiny non-metal has a low Specularity setting and a high Smoothness setting.
    - Smoothness focuses the specular reflection, and the Specular Map controls the amount and color of the specular reflection.
    - The Specular Map can use RGB colors.

## Metals in the Metallic workflow

- The Metallic workflow is simpler, but doesn’t strictly follow the rules of physical light.

- In the Metallic workflow:
    - A shiny metal has a high Metallic setting and a high Smoothness setting.
    - A shiny non-metal has a zero or low Metallic value and a high Smoothness value.
    - Smoothness controls the focus of the specular reflection.
    - The Metallic map only uses grayscale.

![Specular workflow vs. Metallic workflow](References/specular_metallic_comparison.png)

### Which workflow should you use?
- When you import assets, you will see that some use the Specular workflow and others use Metallic. When you have a choice, you can use whichever you prefer. 

- The Metallic workflow is more common because it is easier to work with, but it is not as scientific. 
- The Specular workflow is based on real-world principles of reflectivity, but the coloured specular map makes it more challenging.

## Smoothness (gloss or glossiness)

- brings the specular reflection into focus. 
- from a smooth surface, light reflects in a uniform way so that you can see the shape of the light source in the reflection.

![Specular Workflow](References/specular.png)

![Metallic Workflow](References/metallic.png)