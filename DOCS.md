# CELERIUM DOCUMENTATION
## Content table
- [Overview](#overview)
- [Weak PC Preset](#weak-pc-preset)
- [Installation](#installation)
- [How to add your own files](#how-to-add-your-own-files)
- [Known Issues](#known-issues)
- [Included Mods - What They Do](#how-mods-work)

## Overview
This is the documentation for Celerium, where you can get all the help possible for the modpack. 
It is advised to only be used in case of: 
- Launcher not applying preset configuration from the overrides folder; 
- Explanation of every mod included; 
- Help configuring the video settings your own way. 
Be careful when doing changes to the mods or configurations, if unusure of a setting, leave it as it is.
## Weak PC Preset
This preset is designed for **low-end and older PCs**, including weak CPUs and old integrated GPUs (e.g. Intel HD 3000 / Bay Trail).

---

### Graphics
- Graphics Quality: **Fast**
- Smooth Lighting: **On** (Turn off if desperate or if you need chunks to load faster)
- Weather Quality: **Fast**
- Cloud Quality: **Off**

### Details
- Leaves Quality: **Fast**
- Particles: **Decreased** (or Minimal if you want more performance)
- Biome Blend: **0 blocks**
- Entity Shadows: **Off**

### Performance
- Block Face Culling: **On** (Disable to troubleshoot any performance issues)
- Fog Occlusion: **On**
- Animate Only Visible Textures: **On**
- Chunk Updates: **Soon**  
  *(Use **Deferred** for very old or unstable GPUs)*

### Advanced (Stability-Critical)
- Persistent Mapping: **Off**
- CPU Render Ahead Limit: **0** (Set the Value to 3 to troubleshoot performance issues)

### Important Vanilla Settings
- Render Distance: **6–8 chunks**
- Simulation Distance: **4–6 chunks**

### Preset Variants
- **Weak PC (Safe)**  
  Chunk Updates: **Deferred**, Render Distance: **6**
- **Weak PC (Balanced)**  
  Chunk Updates: **Soon**, Render Distance: **8**

---
  
## Installation

### Manual Installation (Advanced)

This modpack is designed to be installed using a **modpack-aware launcher** such as the **Modrinth App**, **SKLauncher** or **Prism Launcher**.

Manual installation using the **official Minecraft Launcher** is possible, but **not officially supported**, as it does not handle mod dependencies or updates automatically.

If you choose to install manually:
- You are responsible for keeping mods and configs up to date
- Updates must be applied manually
- Support may be limited if issues arise from manual setup

For the best experience and easiest updates, using a supported launcher is strongly recommended.

### Modrinth App (Recommended)

The **Modrinth App** provides the easiest and most reliable way to install this modpack.

1. Install the Modrinth App
2. Search for the modpack on Modrinth
3. Click **Install**
4. Launch the instance once installation is complete

This method automatically handles:
- Mod downloads and dependencies
- Configuration files
- Updates

### Prism Launcher

**Prism Launcher** is a powerful multi-instance launcher suitable for advanced users.

1. Install Prism Launcher
2. Add a new instance \
  2A. Search for the `Celerium` in the Modrinth tab, and choose the version you want
  2B. Import the modpack using the provided `.mrpack` file of your choice
3. Launch the instance after installation finishes

Prism Launcher allows full control over:
- Java versions
- Memory allocation
- Per-instance settings

### SKLauncher

**SKLauncher** supports importing modpacks using both `.zip` and `.mrpack` formats.

1. Open SKLauncher
2. Go to **Modpacks**
3. Click **Import modpack**
4. Select the modpack `.zip` or `.mrpack` file
5. Wait for the import process to complete
6. Launch the modpack from the installation list

While SKLauncher supports modpack importing:
- Dependency handling may vary depending on the pack
- The pack does **not** update automatically
- Some issues may be harder to reproduce compared to modpack-focused launchers

For the most reliable experience and update support, a modpack-aware launcher such as the **Modrinth App** or **Prism Launcher** is recommended. \
If you want any Launcher added in this documentation, talk to me in the ways of contact in the README.

---

## How to add your own files
To add your own files is simple, actually.
1. Go to .minecraft at `C:\Users\[YOUR USER]\AppData\Roaming\.minecraft`
2. If you installed the modpack through a launcher go to A, but if installation was mannual, go to B. \
   2A. In the folder, you will find another folder called ´modpacks´, open that and try to find the folder for Celerium, after you find it, you will have several folders like "mods", "resourcepacks", "shaderpacks", etc. \
   2B. In the folder you will find folders like "mods", "resourcepacks", "shaderpacks", etc.
3. For shaders you put them in the "shaderpacks" folder, resource packs in the "resourcepacks" folder, all of them have their respective folders.
4. Normally, you need a .zip file to put a respective thing in their folder. (Ex.: ComplementaryShaders, SimpleCraft, Fresh Animations, Sodium-extra, etc).
5. Put the .zip file in its respective folder and open the game to test it
  5A. For shader packs, you need to put Iris yourself.

---

## Known Issues
This section lists known issues that may affect some users, along with recommended workarounds where available.

---

### Low FPS or Stuttering on Weak CPUs

On systems with very weak CPUs, occasional stuttering may still occur, especially when:
- Loading new chunks
- Entering dense areas
- Flying quickly

**Workarounds:**
- Reduce **Render Distance** to 6 chunks
- Reduce **Simulation Distance** to 4 chunks
- Set **Biome Blend** to 0
- Close background applications

### GPU Crashes on Older Intel Integrated Graphics

Some older Intel iGPUs (e.g. Bay Trail, HD 3000/4000) may experience crashes or driver resets when using advanced rendering features.

**Workarounds:**
- In Sodium:
  - Set **Chunk Updates** to **Deferred**
  - Disable **Persistent Mapping**
- Use **Fast** graphics settings
- Consider switching to Linux (Mesa drivers tend to be more stable for older Intel GPUs
but do **NOT** if you don't understand how to change Operating Systems, research first.)

### Slow Chunk Loading or Late Terrain Rendering

Chunks may appear slightly later than expected, especially when using safer rendering options.

**Cause:**
This is expected behavior when using **Deferred Chunk Updates**, which prioritizes stability over speed.

**Workaround:**
- Switch **Chunk Updates** to **Soon** if your GPU is stable
- Avoid **Immediate**, as it may cause instability on weak systems

### Visual Pop-in (Leaves, Water, or Lighting)

Visual pop-in can occur due to aggressive culling and fast rendering settings.

**Cause:**
Performance optimizations such as:
- Fast leaves
- Reduced biome blending
- Culling mods

**Workaround:**
This is expected behavior for the Weak PC preset.  
Users with stronger hardware can increase visual settings safely.

### Inconsistent Performance After Updates

After updating the modpack, some users may experience unexpected performance issues.

**Workarounds:**
- Restart the game after updating
- Ensure old config files were replaced correctly
- If issues persist, delete the modpack instance and reinstall

### Manual Installation Issues

Manual installation using the official Minecraft Launcher or unsupported launchers may result in:
- Missing dependencies
- Incorrect configs
- Startup crashes

**Workaround:**
- Use a modpack-aware launcher (Modrinth App or Prism Launcher)
- If installing manually, double-check all mods and configs

If you encounter an issue not listed here, consider reporting it with:
- Your hardware specifications
- Launcher used
- Game and modpack version

## Included Mods – What They Do <a name="how-mods-work"></a>

This modpack focuses on **performance, stability, and usability**, especially for weak or older PCs.  
Below is a brief explanation of what each included mod does.

---

### Better Mount HUD
Improves the HUD when riding mounts by displaying useful information such as mount health and stamina.

### Block Entity Render Distance
Allows limiting how far block entities (e.g. chests, furnaces, signs) are rendered, reducing GPU load.

### Cloth Config API
A library mod required by many other mods to provide in-game configuration screens.

### Debugify
Fixes a large number of vanilla Minecraft bugs, improving stability and correctness without changing gameplay.

### Distant Horizons *(removed after v1.0)*
Adds true distant terrain rendering.  
Removed due to increased CPU and GPU usage, which conflicted with the modpack’s low-end hardware focus.

### Dynamic FPS
Reduces resource usage when Minecraft is in the background or minimized, lowering CPU and GPU load.

### Fabric API
Core library required for most Fabric mods to function.

### Fabric Language Kotlin
Adds Kotlin language support for Fabric mods written in Kotlin. Mostly here to avoid dependency problems if the user adds any mod that needs it.

### FastQuit
Speeds up game shutdown and world exiting, reducing wait times when leaving a world or server.

### FerriteCore
Reduces memory usage by optimizing how Minecraft stores block and item data.

### FPS – Display
Displays the current FPS on-screen for easy performance monitoring.

### ImmediatelyFast
Optimizes immediate-mode rendering, improving UI and overall rendering performance.

### Krypton
Optimizes Minecraft’s networking code, improving multiplayer performance and reducing latency.

### Lithium
Improves game logic performance, including AI, physics, and world ticking, reducing CPU usage.

### Mod Menu
Adds a menu that allows viewing and configuring installed mods directly from the main menu.

### Moonrise
Optimizes chunk loading and scheduling, improving performance during world generation and exploration.

### MoreCulling
Prevents rendering of blocks and entities that are not visible to the player, improving FPS.

### Sodium
A major rendering optimization mod that significantly improves FPS and reduces GPU load.

### Text Placeholder API
Provides placeholder support for text used by other mods (library mod).

### YetAnotherConfigLib (YACL)
Provides a modern and flexible configuration UI used by several mods in the pack.

### Your Options Shall Be Respected (YOSBR)
It's what provides the built-in optimized settings of the pack and keeps it between versions.
