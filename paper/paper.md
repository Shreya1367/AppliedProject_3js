---
title: "Legacy: A Real-Time 3D Animated Movie"
authors:
  - name: Shreya Mishra
    affiliation: 1
  - name: Dr. Tejaswi Gowda
    affiliation: 1
affiliations:
  - name: Arizona State University
    index: 1
date: "2025"
---

# Summary

This project presents the development of *Legacy*, a fully real-time 3D animated movie created using **Three.js**, **motion capture**, and **web technologies**. The goal was to produce a complete short animated film that requires **no offline rendering**, demonstrating how real-time rendering can reduce production time and allow the animation to run directly in a web browser.

The project also explores the creative challenge of transferring **human motion capture** to a **non-human, plant-like character**, revealing how unconventional rigs can be animated effectively.

While many animated films depend on heavy offline rendering pipelines in Blender or Maya, *Legacy* demonstrates that **Three.js** can be a powerful alternative for individuals and students seeking a lightweight, fast, and accessible animation workflow.

# Statement of Need

The traditional 3D film workflow includes long rendering times, complex export pipelines, and heavy reliance on high-performance hardware. Blender and Maya are strong tools for modeling and rigging, but rendering large scenes can take hours or days.

In contrast, **Three.js provides real-time rendering** with several advantages:

- Instant playback — no need to render frames
- Fast iteration on visuals and animation
- Can run on any device with a web browser
- No licensing costs or plugins needed
- Accessible for developers comfortable with JavaScript

This project demonstrates that a visually compelling short film can be produced using a real-time rendering pipeline in just two months, making 3D animation more accessible to individuals and students without access to studio-level render farms.

Additionally, the film’s narrative encourages environmental awareness, symbolized through its plant-like character, and offers an example of applying human mocap to a stylized, non-human rig.

# Process

The production pipeline followed these stages:

## 1. Storyboarding
The visual structure of the film was created using **Storyboarder**.

**Figure 1: Storyboard – Part 1**  
![Storyboard Part 1](figures/fig1.png)

**Figure 2: Storyboard – Part 2**  
![Storyboard Part 2](figures/fig2.png)

## 2. Modeling
Characters and assets were modeled in **Blender**.

**Figure 3: Main Character – Front View**  
![Character Front](figures/fig3.png)

**Figure 4: Main Character – Side View**  
![Character Side](figures/fig4.png)

## 3. Texturing
Textures were downloaded from **Poly Haven**, which provides free CC0-licensed texture libraries and HDRIs.

## 4. Rigging
The character was rigged using:

- **Mixamo** for the body skeleton  
- **FaceIt** for ARKit-compatible facial blendshapes  

## 5. Motion Capture Recording
Motion capture was recorded using:

- Rokoko Face Capture (facial)
- Rokoko Body Capture (full body)
- Export formats: BVH for body, blendshapes for face

## 6. Retargeting and Refining Mocap
The **Rokoko Add-on for Blender** was used to retarget and refine human motion capture onto the non-human character. Multiple motion capture sessions were combined and cleaned for expressive performance.

## 7. Importing into Three.js
Assets were exported to **GLB** format and imported into Three.js. Tasks performed in Three.js included:

- Building scenes based on the storyboard
- Setting up lighting
- Animating cameras
- Sequencing shots
- Real-time rendering with `WebGLRenderer`

This formed the core of the real-time pipeline, allowing the entire film to be sequenced, played, and rendered instantly in a browser.

# Conclusion

*Legacy* demonstrates that **real-time rendering using Three.js** is a practical and efficient alternative to traditional 3D film production. Key conclusions include:

- No final render time is required  
- The film runs instantly in any web browser  
- Blender remains valuable for modeling and mocap retargeting  
- Three.js excels in fast playback and shot sequencing  
- Human motion capture can drive stylized, non-human characters successfully  

The full project, including assets, scenes, and the final film, is available on GitHub:

**[Insert your GitHub]()**
