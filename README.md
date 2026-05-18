# VectArt Animation Add-on

**Author:** Dimona Patrick  
**Version:** 2.0.0  
**Blender Version:** 4.2.0+  
**Category:** Animation  
**License:** GPL-3.0-or-later

## Overview

VectArt Animation is a powerful Blender extension designed to orchestrate expressive, "orchestral" animations for collections of mesh and curve objects. It provides advanced timing, sequencing, collision avoidance, and preset-driven animation styles, all with a modern, clean UI.

## What's New in v2.0.0

- **Modern Extension Architecture**: Fully refactored to use `blender_manifest.toml` (no legacy `bl_info`). Modular codebase split into `properties`, `operators`, `panels`, and `utils` modules.
- **Improved UI/UX**: "Create Animation", "Apply Preset", and "Clear Animation" buttons are now prominently placed in the **main panel** for instant access — no longer hidden inside sub-panels.
- **Blender 4.2+ Best Practices**: Proper type annotations, clean registration/unregistration, SPDX license headers, and adherence to Blender's extension guidelines.
- **Cleaner Code**: PEP 8 compliant, docstrings on all classes and key functions, no dead code.

## Features

- **Collection-Based Animation**: Animate all objects in a collection with a single click.
- **Orchestral Timing**: Control sequencing with delay modes, overlap, randomness, and a unique "Musicality" slider.
- **Animation Presets**: Apply dramatic, cinematic animation styles (Robotic Unfold, Tech Assembly, Explode, etc.).
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
└── utils.py               # Collision detection, timing, preset logic
```

## Usage

### 1. Add Collections
In the **VectArt Animation** panel (View3D > Sidebar > VectArt), add your target collections using the **Add Collection** (+) button.

### 2. Configure Timing
Set Start Frame, Auto Duration, Frames Per Object, and Delay Mode. Adjust the **Musicality** slider for expressive orchestration.

### 3. Choose Animation Style
Open **Style Settings** to select Default or Preset mode:
- **Default mode**: Enable/disable and offset Scale, Rotation, Location, and Extrude animations.
- **Preset mode**: Pick from dramatic animation styles and apply them.

### 4. Create Animation
Click **"Create Animation"** or **"Apply Preset"** directly from the main panel. Use **"Clear Animation"** to reset.

### 5. Advanced Settings
Configure interpolation, easing, velocity, layer order, and local axis in the **Advanced Settings** sub-panel.

### 6. Tools
Use the **Tools** sub-panel for Quick Select, storing original transforms, and keyframe copy/paste operations.

## Animation Presets

| Preset | Description |
|--------|-------------|
| Robotic Unfold | Dramatic scaling, unfolding, and rotation |
| Robotic Transform | Complex, multi-step transformation |
| Tech Assembly | Pieces fly in and assemble with scale and rotation |
| Mech Startup | Mechanical startup with vibration |
| Origami | Complex folding and unfolding animation |
| Holographic | Appear from above with scale and fade |
| Glitch | Random jumps and scale flickers |
| Assemble | Dramatic assembly from all directions |
| Magnetic | Snap-in with bounce |
| Explode | Scale up, explode outward, and fade |

## Support

For bug reports, feature requests, or questions, please open an issue on the [GitHub repository](https://github.com/Dream-Pixels-Forge/add_on_vectart_animation).
