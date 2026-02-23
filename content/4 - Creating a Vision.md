Guess who!

This chapter talks about *Conceptualisation, Data Capturing and Data Processing*, the three steps to, well, creating a visualisation.

# 4.1 Conceptualisation

## Personas
Yep, we're talking about these guys again. If you forgot, they're a method for helping us understand the users, their characteristics and their expectations when using our end product.

In the context of BEV (yeah, finally), we're going to describe a scenario that could trigger the use of our Built Visualisation Environment, in the [[5 - Visualisation Deployment|final deployment format]] (in Chapter 5). We're also gonna need details on our [[2 - Fundamentals of BEV#2.2 Common Reality Capture Methods|Field of View]] (FoV) (in Chapter 2).
<sub>A/N: Future me, you better link these two concepts to their corresponding pages istg.</sub>

The two details we need are:
- Viewing Angles: Single Fixed, or multiple vantage points?
- Viewing distances: Only from up close, or also from a given distance?

These apply to both **2D (360 vids), and 3D (photogrammetry and LiDAR)** reality capture methods. Having good estimates of our FoVs that are needed in the final product **tells us how much of our subject (or environment) needs to be captured**, which **reduces the possibility of needing a reshoot for collecting missing data**, which may not be very practical.

## Flow Chart
Of course, this is not a linear experience. Planning experience like this, based on reality capture, require different approaches.

Storyboards are a basic essential, but something more like a flowchart is "just fantastic". In this context, however the transition between each "state" in this "flow chart" **translates to physical positions in the real world**. That is, like someone moving from a living room to the kitchen, or from point of interest to another, for example. Details from our little puppet Personas will help us in this process?

What do we get from this? **A simple flow-chart with connection nodes (which are the directional arrowheads that link) to clearly identify the possible virtual navigation paths or interaction options that the viewer may take.**

In a way, you can think of this as some sort of "experience map", that dictates the direction of the whole experience. This "forced" thought process facilitates the following:
- Interaction design of our built environment in a straightforward manner (What do you see as you move from Point A to B?)
- Ensures picture continuity in 360 projects, as we capture our source clips in a spatially-logical sequence later on, which keeps our users grounded in both time and space.
	- Basically, it keeps them in a realistically-spaced environment, keeps it kind of 1:1 in our rules of physics in the real world.

**Also, interactive and non-interactive elements should be identified in the flow chart.**

## Consider Limitations
There are two types of important limitations to consider when making our project.
- **Physical**
	- **The presence of physical barriers, obstacles, or constraints may limit or prohibit accessibility.**
	- While we're thinking of our concept, it's good to actually visit the real-life sites to walk around and see if accessibility is, in any way, restricted.
	- For outdoor projects, we should also take note of any spot with harsh lighting or high lighting contrasts at certain times of day. As we'll talk about later (or as you probably already know from how many times it's mentioned in class), consistent lighting without highlights and directional shadows are very good.
- **Legal**
	- **Observe all legal regulations at all times when recording videos.**
	- Locations like museums, national parks and private properties may have local restrictions or conditions regarding imaging and recording.
	- In SG, **the space that unmanned aircrafts (including drones) can fly in is governed by the Civil Aviation Authority of Singapore (CAAS)**. These areas are demarcated as "No-Fly Zones" and "Unmanned Aircraft Flying Areas".

# 4.2 Data Capturing and Processing

This is where the real work's done. *(You'll notice that we didn't talk about LiDAR. Its workflow is nearly identical with Photogrammetry, only being different in data capture)*

## Workflow for 360 Videos
This talks about using a handheld camera, but the same steps would largely apply with a drone.
### 1. Get The Right Camera
- **Cameras should produce vids that can be edited using simple software tools, not requiring laborious stitching or post-processing.**
### 2. Take A Stand
- **Choose a tripod. None of its arms should stick out and show up in the shot.**
	- Travel tripods are ideal due to being lightweight and having an adjustable ball-head.
### 3. Find Proper Placement
- **An omnidirectional camera works best when put in the middle.**
	- With a full headset or cardboard viewer, this lets them turn and look around at anything they want.
	- It's a miracle that this stuff exists, but also means that, being in video-based form, viewers could miss what you're trying to show them.
- **Place the camera somewhere visually stimulating to look at.**
	- Alternatively, give 'em a unique perspective such as a bird's-eye or ant's-eye view.
- **Keep the space between 0.9m to 1.5m from the camera and the subject for best clarity and definition.**
	- 360 Cameras use fisheye lenses. They widen the FoV to capture the whole thing, but also distorts the image.
### 4. Learn Your Moves
- **For Action (moving) shots, keep the camera steady, and limit quick or sudden movements.**
	- If you remember VR, this can cause an unpleasant and shaky experience.
	- Use a gyro or gimbal to keep the horizon steady in these shots.
- **Avoid motion where interaction is planned**
	- 360 vids allow the user to look at whatever they like during playback (or, runtime), but when the camera's moving, they'll lose control of what's in the viewing experience.
	- Something may catch their eye, but if the camera keeps moving, they'll be sort of "fighting" against the momentum to try to look at it.
	- If this continues for long, they'll get tired and just want out.
### 5. Mind The Gap!
- **Avoid filming subjects along the stitch line.**
- A 360 camera is basically two cameras, strapped back to back. Because of this, there's a parallax effect where they meet, a non-congruent place, what we call the "stitch line".
- Software that comes with the cameras usually mitigates this, but it doesn't completely fix it.
- To avoid this, just don't record the main subject of your footage wherever the stitch line is.
### 6. Capture
- **Shoot the subject (with the camera) based on the requirements we made in our Personas and Flow Charts.
- **Ensure color temperature is consistent across all video clips in the set (White balance).**
- **Aim for at least 60 FPS if it's intended to be viewed in VR.**
	- If possible, aim for higher. This is an experimental medium for our users to experience, not just watch.
### 7. Processing (Editing)
- **Trim the clips to remove any unwanted portions (like pressing the record button).**
- **When editing, slow down the 360 video to let the users "explore".
	- If what we have looks great, our audience would wanna look around. This gives them time to do that.
	- Once edited and exported, it'll be ready to be imported to our app for integration.
	- **The workload is doubled when done in stereo.**
- **The most common file format is MP4, using H.264 or H.265 compression, at a suitable bitrate (denoted as bits per second, or bps) for target deployment platform, where you want to deploy it.**

## Workflow for Photogrammetry
This is a good way to make high-res textures and meshes of objects that would otherwise make our lives hell trying to recreate them ourselves in 3D software. It uses digital and smartphone cameras. This one, we should be more familiar with.
### 1. Capture
- **Take a series of overlapping photos of the subject.**
	- 8-megapixel cameras (2010-2013 phones) are enough, but 18-megapixel cameras (~2014 phones) and higher-DSLR-cameras with wide lens are recommended.
	- Fisheye lens will not work, due to aforementioned distortion.
	- Do not capture everything. Select a subset or list of assets to make the process more efficient.
- **Take photos sequentially around the subject.**
	- Start with taking them in a circle at a low angle, then do another at a high angle. Take another few for the important details.
	- Assets that appear nearer to the virtual camera in our 3D environment will need higher resolutions that background assets. Basically, if they're closer to us, they'll need more detail.
- **Aim for 50-60% overlap in pictures; 60-80% is ideal.**
	- Between each shot, do a 30cm sidestep.
	- Don't move when taking a pic, or you'll end up with blurry pictures.
- **Make sure object surfaces are matte.**
	- Transparent objects will not convert well, as I'm sure you know by now.
	- Reflective surfaces can be converted to matte with dry shampoo spray (huh, that's neat).
- **Ensure color temperature is consistent across all video clips in the set (White balance).**
	- Haven't I seen this before...?
- **Lighting has to be consistent throughout the shot, optimal on cloudy days.**
	- During a sunny day, outdoor environments will have highlights and directional shadows that would be hard to remove.
	- **De-Lighting, a light removal step.**
		- If you want an asset to work in any lighting condition, this is required to remove harsh lighting info baked in. It also helps with making the textures tileable, which means they can be seamlessly repeated.
- **For a small space or object, 40-50 photos is enough.**
	- Of course, more photos is better.
	- However, more photos also equals more processing time. Focus on quality instead of quantity of captures.
- **Never move the subject during a shoot.**
	- Self-explanatory, perhaps. Just don't do it.
- **Focus the camera on the subject for every shot.**
	- All photos must be sharp and clear.
- **Use a tripod to reduce motion blur.
	- Also good for low-lit environments that need higher exposure time.
### 2. Upload
- **Import your photos to your photogrammetry software.**
	- This should be an easy drag-and-drop.
### 3. Generate the 3D Model (Point Cloud and Texture Data)
This part is done automatically. Let's run through it.
- **Image matching**
	- The software algorithm finds the overlaps between images and stores how they'll all be stiched.
- **Feature extraction**
	- It combs through the photos for features that are present across multiple images.
	- Quality can be increased by increasing keypoint sensitivity and matching ratio, changing presets and switching matching algorithms.
- **Triangulation**
	- 3D coordinates of the surface points are estimated based on the output of the earlier extraction. If it finds a spatial group of pixels with enough similarities, it makes a point.
	- The result is our beloved Point Cloud.
- **Texture**
	- Color information is transferred to either the mesh's vertex colors (colorise) or to textures used on the surface of the mesh. Initial UVs are created by the reconstruction software.

### 4. Post-Processing
This is the real work, after our point cloud is generated. Of course, what the software creates is not ready for use immediately. We need to clean it up with a **correct orientation, pivot and UV set.**

- **Clean Up**
	- Usually, there are floating artifacts, background noise, holes and stuff to clean up before we can actually export a lower-res mesh
- **Mesh Retopology**
	- **Retopology is simplifying the topology of a mesh to make it cleaner and easier to work with.**
	- The mesh we're gonna get will look divine with an insane amount of detail. Unfortunately, putting that in the middle of the game or a 3D experience is not a good idea.
	- It's needed for the mangled topology resulting from sculpting or generated topology, like a 3D scan.
	- If the mesh is going to be deformed in some way, like a cloth or a soft body, this step is needed.
	- It can be done hand-by-hand, manipulating geometry using editing tools. It can also be done automatically with methods that some photogrammetry or third-party software provide.
- **Texture Baking**
	- After retopology, we're gonna get a new, lower-polygon mesh with a new UV set.
	- Any corresponding textures are gonna have to go through a "baking" process to transfer the texture's color info based on the new UV.
- **Scale and Orientation**
	- The object will be rescaled and reoriented. May be done arbitrarily by the software.
- **Export 3D Mesh**
	- Most software for this kind of thing comes with the clean-up tools for what we talked about above.
	- After that, you can export the point cloud into a 3D mesh format like OBJ (3D Mesh only) or FBX (3D Mesh and Texture file), compatible with 3D software and game engines.
	- Some apps might even let you export with different texture resolutions and corresponding textures for use with Level of Detail (LoD) setups typically found in Unreal or Unity.
	- Yeah, remember LoDs? If not, they lower the mesh's detail when viewed from far away, good for optimisation
## Having Trouble with Photogrammetry?
These tips are guaranteed to help you get started in no time! This is not financial advice.

### Full Coverage
**When shooting an object (again, with your camera), it's important to have full coverage of it.** All parts of the object must be covered by several photos so the program can figure out what its looking at, and can create groups of similar pixels for a final asset without holes or under-sampled areas.

You can take many far shots, and then some closer ones to provide more detail. At each horizontal camera location, make sure you cover the subject vertically.

To be honest, this can be difficult. It's easy to miss some elements during the shooting. If you should, then absolutely take more photos and even put them through a test run on site in your software.

### Reuse Where Possible
Small or individual objects are often used to populate areas where there are a lot of them by duplicating them around in different areas, like office chairs in a meeting room.

If variety is needed, you can scale, rotate and mirror them. For these kinds of objects, you'll need to cover all parts from all directions to reconstruct full assets.

### Bad Candidates for Photogrammetry
These are:
- Moving subjects (foliage in the wind)
- Shiny or Reflective surfaces (metallic or wet surfaces)
- Transparent surfaces (glass)

As well, if the object has large, flat areas of color, the software won't have enough info to distinguish groups of similar pixels as, well, they all look the same with the same color.

To help the software along, you can try painting on the objects or projecting fixed light patterns. If you do, though, only geometry will be extracted, and the textures are gonna have to be produced separately.

If your object is **too flat-colored** for the software to reconstruct, you'll end up with **multiple point clouds, not good**. If it has **distinct features**, it will have **one point cloud, very good**.

## Full Photogrammetry Workflow, by Unity Technologies
And finally, take this model.
![[Pasted image 20260223214137.png]]

---
[[5 - Visualisation Deployment|Next]] || [[3 - Fundamentals of 3D|Prev]]<br>
[[0 - Index|Index]]

And wow! That's it from me!

That's the last chapter I'll ever write for the Skeleton Book in ITE. Crazy, how that feels.

Anyway, Jeb'll be back to send this module off. I'll write my sappy goodbye in the index, because I like sappy goodbyes. I'll recommend finishing off chapter 5 first, then you can go back and read it.

If there's nothing else, I guess I'll see you 'round!
