
# 2.1 What is a Built Environment?

A built environment consists of **physical man-made surroundings** where people live, learn, work, and play. It is the opposite of a natural environment where living and non-living things naturally exist.

***4 Common Types of Built Environment:***

• **Industrial:**
Found in large, centralised hubs; often noisy, densely populated, and often used for manufacturing and other industrial activities that require a lot of space.

• **Retail:**
Located in commercial areas like shopping malls; designed for a **comfortable and convenient shopping experience for customers**.

• **Residential:**
Found in suburban areas and new housing developments; designed for a comfortable, safe, and convenient lifestyle for residents.

• **Commercial:**
Structures and Features used to **generate revenue**, such as office buildings and factories.

---
# 2.2 Common Reality Capture Methods

Reality Capture is the process of **digitally capturing, analysing, and representing the physical world** as immersive experiences.

1. **360° Videos (2D):**
   Filmed omnidirectionally to cover the entire surroundings (360-degree horizontal and 180-degree vertical view).

   **FOV(Field of View):**
	   An important aspect to consider when discussing the viewing range of 360 cameras. **It is a term in photography that refers to the extent of the scene that a camera can capture (the “observable area”).**

	  **Many 360 video authoring platforms require your input source to be in the Equirectangular format.**


Pros:
- **Low entry barrier.**
- **Because of its immersive quality, 360 videos can help the viewer to connect with the content in a meaningful and emotional way.**
- **360 videos easily translate into Virtual Reality (VR) experiences when ported to dedicated VR headsets.**

Cons:
- **Since it is essentially a video recording, you have to rely heavily on single takes (It is hard to hide video cuts).**
- **Limited video resolutions with current technology commonly result in relatively poorer or lower end quality.**
- **May involve labour-intensive video editing process.**

  **Stereoscopic 360:**
  **Provides a perspective for each eye to create depth and separating objects from the foreground and background**, often requiring both left and right eye videos be displayed in the same video container, which halves the resolution in the viewport. Often requiring 3D glasses or a headset.

  **Stereoscopic 180:**
  **Stereo 3D Content for only the front 180 degrees** and great for content that has most of the action facing the front, and several platforms can take advantage of not needing to display the rear pixels which allows for higher resolutions. Often requiring 3D glasses or a headset

  **Mono 360:**
  **A 360 Video without 3D depth**. It is the most cost-effective content to shoot, and can be streamed at higher resolutions since it is only a single channel. It can also be more forgiving when shooting mono, allowing for easier stitching on objects closer to the camera.

2. **Photogrammetry (2D to 3D):**
  Photogrammetry is **a process to obtain, record, interpret, and replicate accurate information about three-dimensional (3D) physical objects using two-dimensional (2D) photographs.**
   Two general types of photogrammetry exist: **Aerial** (e.g. drones) and **Terrestrial** (e.g. handheld camera or on a tripod). The resultant data output from a Photogrammetry process is called a “Point Cloud”.

**Advantages** of Photogrammetry:
- **Non-intrusive to the physical objects being photographed.**
- **High level of accuracy in visual detail can be achieved.**
- **Cost-effective and time-saving.**

**Disadvantages** of Photogrammetry:
- **For Terrestrial photogrammetry, the camera operator's photography skills are essential.**
- **Quality is heavily affected by ambient (surrounding) light conditions.**
- **Requires clear unobstructed line of sight to target objects that need to be static (non-moving) throughout data acquisition (photographing) process.**

3. **LiDAR(3D):**
   LiDAR (Light Detection and Ranging) is **a remote sensing method by measuring the time taken for laser beams to reflect from the target object.** It **creates a 3D scan by mapping an object, structure, or area, and describing it in the form of x, y, and z coordinates in a format** known as a “Point Cloud".

Advantages of LiDAR:
- **Surface data has a higher sample (resolution) density, as compared to the other methods.**
- **Unaffected by lighting conditions for model generation, improving efficiency.**
- **Minimum human dependence since capturing process is mostly automated.**

Disadvantages of LiDAR:
- **Does not work with reflective surfaces, such as glass and mirrors.**
- **More expensive ($) as compared with the other methods.**
- **Large datasets collected require longer time to analyse and to process.**

---
# 2.3 Colour Temperature

**Colour temperature** refers to the degree of warmness or coolness of visible light, measured in **degrees Kelvin (K)**.

• **White Balance:** The setting that makes **white look white**, as opposed to having a blue or orange tint. Consistency is vital for Reality Capture processing; otherwise, post-processing is needed to colour-correct the image set.

**Implications on Reality Capture:**
**It is important for captured images to look consistent in colour temperature for Reality Capture processing.** Therefore, we need to pay attention to the “White Balance” settings in digital imaging hardware for 360 Videos and Photogrammetry. Very simply, the **White Balance setting on your camera should correspond to the lighting situation you are in.** Otherwise, separate additional post-processing of images may be necessary to colour-correct the entire image set for consistency.

---
[[3 - Fundamentals of 3D|Next]] || [[1 - Persona (5 Royal)|Prev]]<br>
[[0 - Index|Index]]
