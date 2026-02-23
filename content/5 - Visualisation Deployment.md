Sup I'm back! After 4 Chapters we are finally on the last chapter...**Visualisation Deployment**!
# 5.1 Think About Your Deployment Strategy Upfront

It might seem weird to talk about the end at the beginning, but **you should start thinking about deployment from the very beginning of your project**. How your audience consumes the content has a huge impact on how you decide to **"capture"** your project in the first place.

***Deployment Options:***

• **Demo in Person:** Many brands show content face-to-face at **tradeshows or sales meetings**. Content is typically **side-loaded** to a device, giving you complete control over the display on a desktop, mobile, or VR headset.

• **Social Media Platforms:**

   ◦ **360 Videos:** Upload to **TikTok, YouTube, Facebook, or Vimeo**. There are also VR-targeted platforms like **Samsung VR, Rad.live, and VeeR VR** where users view content in headsets.

   ◦ **3D Models:** Use generic sites like **Sketchfab, ArtStation, or Thingiverse**, but keep in mind that interactivity is usually **very limited** to basic display only.

• **Custom Application Development:** Build your own VR or 3D apps using engines like **Unreal or Unity**. This makes your brand more discoverable on app stores and opens up a world of **interactivity** beyond a linear video experience.

• **App Platforms (360 only):** Frameworks like **Viar360 or InstaVR** allow for easy distribution across various headsets, though they might limit your ability to customize.

--- 
# 5.2 Technical Specs and Online Deployment

When going online, remember that not all platforms are equal—some might not support **stereoscopic 3D or spatial audio**.

***The Bandwidth Battle:***

1. **Live streaming 360 content** is process and **bandwidth intensive**. You are often **"at the mercy of upload speed"** at the user's location and their internet quality.

2. **Bitrates** (denoted by **"bits per second," or bps**) have to be kept low to prevent buffering.

3. **H.265 (HEVC):** This codec is a hero because it can provide **"comparable quality level at half the bitrate of a H.264 video"**.



***Interactivity & Web Standards:***

1. **Branching Narratives:** You can move beyond linear experiences by allowing viewers to **change the outcome of the story** based on their decisions.

2. **Training Modules:** These can **track a viewer's attention** to ensure they focus on the most important parts of a process.

3. **WebVR:** These standards make it easier to integrate VR directly into browsers like **Chrome and Firefox**, paving the way for easy deployment without needing a separate app.

---
# 5.3 Export Formats, Testing and Debugging

To make sure your project actually works on your target platform, you've got to use the right recipes.

| <font color="#ff0000">Content Type</font> | <font color="#ff0000">File Export Format(s)</font> |
| ----------------------------------------- | -------------------------------------------------- |
| **360 Still (2D)**                        | **JPEG (.jpg)**                                    |
| **360 Videos (2D)**                       | **H.264 or H.265 (.mp4 or .mov)**                  |
| **3D Models (Meshes)**                    | **OBJ or FBX (.obj or .fbx)**                      |

Testing & Debugging (The "Look out for" List)

Before you launch, put on your detective hat and check these attributes:

• ***For 360 Content:***

   ◦ **Picture Continuity:** Ensure clips form a **"spatially logical sequence"** so viewers don't feel "lost".

   ◦ **Hotspots:** Check that this **"linkage function"** is correctly connecting your clips.

   ◦ **Visuals:** Maintain consistent **colour temperature** and correct resolution/bitrate.

• ***For 3D Models:***

   ◦ **The Big Three:** Ensure models are in the correct **position, orientation, and scale**.

   ◦ **Colliders:** Add a **collision (or collider) node** so users can't **"pass through"** objects. This is also required for physics simulations.

   ◦ **Polish:** Verify textures display properly, **LOD models** are set up, and no **polygon faces** are missing or **inverted** (facing the wrong side).

---
[[4 - Creating a Vision|Prev]]
[[0 - Index|Index]]

That brings us to the end of this chapter and with it, the final skeleton book in the series.
It has been a pleasure and it certainly was a fun journey. Safe travels everyone!

"Can't let this go 'cause I'm always gonna be a dreamer" - Last Dinosaurs