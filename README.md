# Ways to Render 1 Million Cubes
All the ways to efficiently render 1 Million cubes in Unity3d (I could think of).
**WIP: This repository will be filled with implementation over time**

## ECS 

<br/>

## Instanced Rendering

### Using MeshRenderers & MaterialPropertyBlock
#### Description
### Using DrawMeshInstanced
#### Description
### Using DrawMeshInstancedIndirect
#### Description
_Using a single Mesh Instance, a single Material Instance and a custom shader accepting arbitrary StructuredBuffers (like positions,rotations,colors, etc) and triggering the instanced drawing by calling the [Graphics.DrawMeshInstancedIndirect](https://docs.unity3d.com/ScriptReference/Graphics.DrawMeshInstancedIndirect.html) on every frame. The shader should be written to care of the translation/scale/rotation of each instance._
#### Benefits
* Arbitrary meshes can be used
* Sub-meshes can be instanced separately
* The transformation matrix for each element of the grid could be defined entirely on the shader

<br/>

## Procedural Meshing

### Generating the Cubes as a single Mesh
#### Description
### Generating the Cubes using a Geometry Shader
#### Description


<br/>

## Raymarching

### Using a repeating Cube Signed Distance Field
#### Description
### Using a Volumetric RenderTexture
#### Description

