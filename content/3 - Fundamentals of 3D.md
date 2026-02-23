 Hiya it's me again!

# 3.1 What happens next after Reality Capture?

Methods like Photogrammetry and LiDAR output data known as **“Point Clouds,”** which are **discrete sets of data points in space representing a 3D shape or object.** These must be converted and optimised into lower resolution 3D mesh surfaces called **“3D models”** to be interpreted by game engines like Unreal or Unity.

# 3.2 Important 3D Modelling Concepts


• **Vertex:**
A single point and the smallest component of a 3D model.

• **Edge:**
A straight line that connects two vertices and defines the model's shape.

• **Polygon:**
Any shape formed by connecting straight lines.

• **Face:**
The most basic part of a polygon mesh; the space formed between connected edges.

• **Mesh:**
A collection of polygons connected along their edges.

• **Topology:**
Refers to how the components of a mesh are distributed and connected.

• **Normals:**
A vertical line jutting out of each face is called a “Normal”. It is important for all the faces of a 3D model to be **facing the correct orientation (usually outwards and single-sided only) with no overlaps** so that they will render (display) properly in real-time engines. The direction of the face determines how light should behave on that particular face in real-time engines.

• **UVs:**
2D texture coordinates that reside with the vertex information for polygonal surface meshes. They provide the connection between the surface mesh and how the image texture gets mapped onto it.

• **Textures:**
A **bitmap image** applied to the surface of 3D objects to add detail and realism.

• **Materials:**
Define how mesh surfaces react to virtual lights. Simple materials consist of a single flat colour; complex ones include multiple textures and physically-based shading.

• **Pivot Points:**
The position around which objects or components are moved, rotated, and scaled. By default, the pivot point is located at the object's centre. **You need them for accurate manipulation and placement in 3D applications.**

---
[[4 - Creating a Vision|Next]] || [[2 - Fundamentals of BEV|Prev]]<br>
[[0 - Index|Index]]
