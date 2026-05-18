# VectArt Animation Add-on

**Author:** Dimona Patrick  
**Version:** 2.1.0  
**Blender Version:** 4.2.0+  
**Category:** Animation  
**License:** GPL-3.0-or-later

## Overview

VectArt Animation is a powerful Blender extension designed to orchestrate expressive, "orchestral" animations for collections of mesh and curve objects. It provides advanced timing, sequencing, collision avoidance, preset-driven animation styles, and **procedural Geometry Nodes animation**, all with a modern, clean UI.

## What's New in v2.1.0

- **Geometry Nodes Animation Mode**: Apply procedural GN effects (Wave Deform, Noise Displacement, Dissolve, Scatter Grow, Smooth Inflate) with auto-keyframed inputs.
- **5 New Animation Presets**: Typewriter, Spiral In, Bounce Drop, Elastic Pop, Domino Fall.
- **Improved Existing Presets**: All original presets refined with more steps, smoother transitions, and better overshoot/settle behavior.
- **One-Click GN Remove**: Easily strip all VectArt GN modifiers and clean up unused node groups.

## Features

- **Collection-Based Animation**: Animate all objects in a collection with a single click.
- **Orchestral Timing**: Control sequencing with delay modes, overlap, randomness, and a unique "Musicality" slider.
- **15 Animation Presets**: Apply dramatic, cinematic animation styles with improved multi-step sequences.
- **Geometry Nodes Animation**: 5 procedural GN presets that create node groups with keyframed inputs for mesh deformation effects.
- **Collision Avoidance**: Smart placement to prevent object overlap during animation.
- **Grid-Based UI**: Clean, organized panels for timing, style, and advanced settings.
- **Keyframe Tools**: Copy, paste (including reverse), and clear keyframes for batch workflows.
- **Customizable Animation Types**: Combine scale, rotation, location, and extrude animations with per-type offsets.
- **Advanced Easing & Interpolation**: Multiple interpolation and easing types for professional results.
- **Layered Animation Order**: Animate top-down, bottom-up, or simultaneously.
- **Quick Select & Management**: Easily manage and select objects/collections for animation.

## Installation

1. Download the `add_on_vectart_animation.zip` from this repository.
2. In Blender, go to **Edit > Preferences > Get Extensions** (or install via drag-and-drop in Blender 4.2+).
3. Install the `.zip` file.
4. Enable **VectArt Animation** in the extensions list.

## File Structure

```
add_on_vectart_animation/
├── blender_manifest.toml   # Extension metadata (replaces bl_info)
├── __init__.py             # Entry point — registers sub-modules
├── properties.py           # All PropertyGroup definitions
├── operators.py            # All Operator definitions
├── panels.py              # All Panel and UIList definitions
├── utils.py               # Collision detection, timing, preset logic
└── geometry_nodes.py      # Procedural GN animation presets
```

## Usage

### 1. Add Collections
In the **VectArt Animation** panel (View3D > Sidebar > VectArt), add your target collections.

### 2. Configure Timing
Set Start Frame, Auto Duration, Frames Per Object, and Delay Mode. Adjust the **Musicality** slider for expressive orchestration.

### 3. Choose Animation Mode

#### Default Mode
Enable/disable and offset Scale, Rotation, Location, and Extrude animations.

#### Preset Mode
Pick from 15 dramatic animation styles and apply them with one click.

#### Geometry Nodes Mode (NEW)
Select a procedural GN preset and apply it to mesh objects. The addon creates a geometry node group with animated inputs — no manual node wiring needed.

### 4. Create Animation
Click **"Create Animation"**, **"Apply Preset"**, or **"Apply GN Effect"** directly from the main panel.

### 5. Advanced Settings
Configure interpolation, easing, velocity, layer order, and local axis.

## Animation Presets

| Preset | Description |
|--------|-------------|
| Robotic Unfold | Multi-step unfolding with scale/rotation |
| Robotic Transform | Complex multi-axis transformation |
| Tech Assembly | Fly-in assembly with snap-to-place |
| Mech Startup | Mechanical startup with bounce vibration |
| Origami | Complex folding and unfolding |
| Holographic | Scan-line appearance from above |
| Glitch | Random teleport with scale flickers |
| Assemble | Dramatic assembly from scattered pieces |
| Magnetic | Snap-in with bounce overshoot |
| Explode | Scale up, scatter outward, fade |
| **Typewriter** | Quick stamp-in like typewriter keys |
| **Spiral In** | Spiral inward with rotation |
| **Bounce Drop** | Drop with squash-stretch bounce |
| **Elastic Pop** | Pop-in with elastic overshoot |
| **Domino Fall** | Sequential domino-style topple |

## Geometry Nodes Presets

| GN Preset | Description |
|-----------|-------------|
| Wave Deform | Animated sine-wave deformation along geometry |
| Noise Displacement | Procedural noise-driven vertex displacement |
| Dissolve | Progressive random face deletion |
| Scatter Grow | Animated particle scatter growing on surface |
| Smooth Inflate | Smooth spherical inflation/deflation |

## Support

For bug reports, feature requests, or questions, please open an issue on the [GitHub repository](https://github.com/Dream-Pixels-Forge/add_on_vectart_animation).
