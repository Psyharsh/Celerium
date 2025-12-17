# CELERIUM DOCUMENTATION
## Content table
- [Overview](#overview)
- [Weak PC Preset](#weak-pc-preset)
- [Installation](#installation)
- [Known Issues](#known-issues)
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
- Smooth Lighting: **Off** 
- Weather Quality: **Fast**
- Cloud Quality: **Off**
- Sky Rendering: **Off**
- Stars: **Off** (optional)
- Sun & Moon: **Off** (optional)
- Fog: **Fast**

---

### Details
- Water Quality: **Fast**
- Leaves Quality: **Fast**
- Particles: **Decreased** (or Minimal if you want more performance)
- Rain Splash: **Off**
- Biome Blend: **0 blocks**
- Entity Shadows: **Off**

---

### Performance
- Block Face Culling: **On** (Disable to troubleshoot any performance issues)
- Compact Vertex Format: **On**
- Fog Occlusion: **On**
- Animate Only Visible Textures: **On**
- Always Defer Chunk Updates: **Off**
- Chunk Updates: **Soon**  
  *(Use **Deferred** for very old or unstable GPUs)*

---

### Advanced (Stability-Critical)
- Multidraw: **Off**
- Persistent Mapping: **Off**
- CPU Render Ahead Limit: **0**
- Allow Direct Memory Access: **Off**

---

### Important Vanilla Settings
- Render Distance: **6–8 chunks**
- Simulation Distance: **4–6 chunks**

---

### Preset Variants
- **Weak PC (Safe)**  
  Chunk Updates: **Deferred**, Render Distance: **6**
- **Weak PC (Balanced)**  
  Chunk Updates: **Soon**, Render Distance: **8**
  
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

---

### Prism Launcher

**Prism Launcher** is a powerful multi-instance launcher suitable for advanced users.

1. Install Prism Launcher
2. Add a new instance
3. Import the modpack using the provided `.mrpack` file
4. Launch the instance after installation finishes

Prism Launcher allows full control over:
- Java versions
- Memory allocation
- Per-instance settings

---

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
- Automatic updates are not guaranteed
- Some issues may be harder to reproduce compared to modpack-focused launchers

For the most reliable experience and update support, a modpack-aware launcher such as the **Modrinth App** or **Prism Launcher** is recommended. \
If you want any Launcher added in this documentation, talk to me in the ways of contact in the README.

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

---

### GPU Crashes on Older Intel Integrated Graphics

Some older Intel iGPUs (e.g. Bay Trail, HD 3000/4000) may experience crashes or driver resets when using advanced rendering features.

**Workarounds:**
- In Sodium:
  - Set **Chunk Updates** to **Deferred**
  - Disable **Multidraw**
  - Disable **Persistent Mapping**
- Use **Fast** graphics settings
- Consider switching to Linux (Mesa drivers tend to be more stable for older Intel GPUs)

---

### Slow Chunk Loading or Late Terrain Rendering

Chunks may appear slightly later than expected, especially when using safer rendering options.

**Cause:**
This is expected behavior when using **Deferred Chunk Updates**, which prioritizes stability over speed.

**Workaround:**
- Switch **Chunk Updates** to **Soon** if your GPU is stable
- Avoid **Immediate**, as it may cause instability on weak systems

---

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

---

### Inconsistent Performance After Updates

After updating the modpack, some users may experience unexpected performance issues.

**Workarounds:**
- Restart the game after updating
- Ensure old config files were replaced correctly
- If issues persist, delete the modpack instance and reinstall

---

### Manual Installation Issues

Manual installation using the official Minecraft Launcher or unsupported launchers may result in:
- Missing dependencies
- Incorrect configs
- Startup crashes

**Workaround:**
- Use a modpack-aware launcher (Modrinth App or Prism Launcher)
- If installing manually, double-check all mods and configs

---

If you encounter an issue not listed here, consider reporting it with:
- Your hardware specifications
- Launcher used
- Game and modpack version
