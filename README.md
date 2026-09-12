# 🏗️ Plinthes Fred - Modified Version v1.11.0

**Blender 5.2 Addon** to automatically generate **baseboards**, **door frames** and **window frames**.

![Version](https://img.shields.io/badge/Version-1.11.0-blue)
![Blender](https://img.shields.io/badge/Blender-5.2+-orange)
![Python](https://img.shields.io/badge/Python-3.10+-green)
![License](https://img.shields.io/badge/License-GPL-red)

---

## 📋 Overview

**Plinthes Fred** is a powerful Blender addon that automatically generates:

- ✅ **Baseboards** - Professional moldings at the base of walls
- ✅ **Door Frames** - Door encasements with customizable jambs
- ✅ **Window Frames** - Window encasements with sills and jambs

All shapes are generated from selected geometry with advanced options to customize appearance.

### Modified Version

This version has been **simplified** by removing:
- ❌ **Unwrap** (UV Management)
- ❌ **Material** (Material Application)
- ❌ **Advanced** (Advanced Parameters)

**The essential features remain 100% functional** ✅

---

## 🎯 Main Features

### Baseboard

Generates baseboards along walls with:
- **Multiple profiles** (Square, Chamfer, Bullnose, Cove, Ogee, Stepped)
- **Automatic mitered corners**
- **Height and depth adjustment**
- **Automatic smooth shading**

### Door Frame

Creates door encasements with:
- **Customizable profiles**
- **Optional jamb lining**
- **Proper corner treatment**
- **Two sides possible** (interior/exterior)

### Window Frame

Generates window frames with:
- **Multiple profiles**
- **Customizable sill (rebord)**
- **Jamb lining**
- **Mitered corners**

---

## 🚀 Installation

### Prerequisites

- **Blender** 5.2.0 or higher
- **Python** 3.10+ (included with Blender)
- System: Windows, macOS, or Linux

### Steps

#### 1. Download

Download `plinthes_byfred_modified.zip`

#### 2. Extract

Extract the ZIP file → you get the `plinthes_byfred_final` folder

#### 3. Locate the Blender Addons Folder

**Windows:**
```
C:\Users\[USERNAME]\AppData\Roaming\Blender Foundation\Blender\5.2\scripts\addons
```

**macOS:**
```
/Users/[USERNAME]/Library/Application Support/Blender/5.2/scripts/addons
```

**Linux:**
```
/home/[USERNAME]/.config/blender/5.2/scripts/addons
```

#### 4. Copy the Folder

Copy `plinthes_byfred_final` into the addons folder

#### 5. Restart Blender

Close and restart Blender completely

#### 6. Enable the Addon

1. Open **Preferences** (Edit > Preferences)
2. Go to **Add-ons**
3. Search for **"plinthes"** or **"fred"**
4. Check the box to enable

✅ **The addon is ready to use!**

---

## 📖 User Guide

### Access the Addon

The addon adds a panel in:
```
View3D > Sidebar (N) > plinthes fred
```

### General Interface

#### Available Panels

**For Baseboard:**
- 📋 **Main** - Type and mode selection
- 📏 **Size** - Dimensions (height, depth, etc.)
- 🎯 **Fit** - Wall adjustment
- 🎨 **Shading** - Shading and smoothing

**For Door Frame:**
- 📋 **Main** - Type and configuration
- 📏 **Size** - Frame dimensions
- 🚪 **Jamb** - Jamb options
- 🎨 **Shading** - Shading

**For Window Frame:**
- 📋 **Main** - Type and configuration
- 📏 **Size** - Dimensions
- 🪟 **Sill** - Customizable sill
- 🚪 **Jamb** - Jamb lining
- 🎨 **Shading** - Shading

---

## 📝 Typical Workflow

### Create a Baseboard

#### Step 1: Select Faces

1. Enter **Edit Mode** (Tab)
2. Select **the bottom faces of the walls**
3. Exit edit mode (Tab)

#### Step 2: Create the Baseboard

1. Open the **plinthes fred** panel (View3D Sidebar)
2. Click **"Create Baseboard"**
3. The baseboard is generated immediately

#### Step 3: Adjust (Optional)

1. Modify the parameters:
   - Height
   - Depth
   - Profile type
   - Corners
2. The baseboard updates **in real-time** ✨

#### Step 4: Finalize

1. Click **"Rebuild"** to confirm
2. The baseboard is ready to export

### Create a Door Frame

#### Step 1: Select the Opening

1. Enter **Edit Mode** (Tab)
2. Select **the perimeter of the opening**
3. Exit edit mode (Tab)

#### Step 2: Create the Frame

1. Open the **plinthes fred** panel
2. Click **"Create Door Frame"**
3. The frame is generated

#### Step 3: Customize

Adjust the parameters:
- Width and depth
- Profile
- Jamb lining
- Sides (interior/exterior)

### Create a Window Frame

Same process as door frame, with additional options for sill customization.

---

## ⚙️ Available Parameters

### Baseboard - Size

| Parameter | Description |
|-----------|-------------|
| **Height** | Baseboard height |
| **Depth** | Depth (thickness) |
| **Base Depth** | Base depth |
| **Crown Height** | Height for crowns |

### Baseboard - Fit

| Parameter | Description |
|-----------|-------------|
| **Profile** | Profile type (Square, Bullnose, etc.) |
| **Segments** | Number of curve segments |
| **Corners** | Corner type (Miter, Butt, Bevel) |
| **Angle** | Corner angle |

### Shading (All Panels)

| Parameter | Description |
|-----------|-------------|
| **Shade Smooth** | Enable smooth shading |
| **Smooth Angle** | Angle for auto-smooth |
| **Auto Smooth** | Automatic activation |

---

## 🎨 Available Profiles

### Baseboard Profiles

- **SQUARE** - Simple and flat
- **CHAMFER** - 45° bevel
- **BULLNOSE** - Convex rounded
- **COVE** - Concave rounded
- **OGEE** - Ogival profile
- **STEPPED** - Stepped

### Door/Window Profiles

Same range as Baseboard, adapted for encasements.

---

## 🔧 Troubleshooting

### Addon doesn't appear

**Verify:**
- Blender 5.2+ is used ✓
- The folder is in the correct location ✓
- Blender has been completely restarted ✓
- In Preferences > Add-ons, check the addon ✓

**Check for errors:**
1. Open console (View > Toggle System Console on Windows)
2. Restart Blender
3. Observe error messages

### Generations don't display

**Verify:**
- You are in **Edit Mode** when selecting
- Selected faces/edges are valid
- Display mode allows viewing new objects

### Parameters don't update

**Solution:**
1. Click **"Rebuild"** after each modification
2. Verify that the baseboard object is selected

### Python error on startup

**Verify:**
- Blender version is **5.2.0+**
- No other version of this addon is enabled

---

## 📊 Advanced Features

### Source Objects

The addon creates a **direct link** with source walls:
- Modify walls → baseboards update
- Use **"Rebuild"** to regenerate

### Presets

Save your preferred configurations:
1. Configure parameters
2. Click **"Save Preset"**
3. Load later with **"Load Preset"**

### UV and Materials

⚠️ **Note:** This modified version does not include Unwrap and Material panels.
- For UV: use standard Blender tools
- For materials: apply manually after generation

---

## 🆘 Support & Feedback

### Documentation

- Read this README completely
- Try basic examples
- Consult available settings

### Resources

- **Blender Manual**: https://docs.blender.org
- **Python API**: https://docs.blender.org/api/current/

### Report a Bug

If you encounter an issue:
1. Note exact steps to reproduce
2. Check Blender console for errors
3. Verify Blender 5.2+ is used

---

## 📝 License

**Plinthes Fred** is provided under **GPL v3** license.

- ✅ Personal and commercial use authorized
- ✅ Code is modifiable
- ✅ Redistributable under the same license

---

## 🔄 Modifications in This Version

### Modified Version v1.11.0

This version is **based on plinthes fred v1.11.0** with modifications:

**Removed:**
- ❌ Panel `VIEW3D_PT_trim_*_unwrap` (Unwrap)
- ❌ Panel `VIEW3D_PT_trim_*_material` (Material)
- ❌ Panel `VIEW3D_PT_trim_*_advanced` (Advanced)

**Preserved:**
- ✅ All generation features (100%)
- ✅ All profiles
- ✅ All Size/Fit/Jamb/Sill parameters
- ✅ Automatic shading

---

## ✨ Advantages

✓ **Fast generation** - Create baseboards in seconds
✓ **Real-time updates** - Modify parameters, baseboard changes immediately
✓ **Multiple profiles** - 6 built-in profile types
✓ **Smart corners** - Automatic miter corner handling
✓ **Automatic shading** - Smoothing applied correctly
✓ **Intuitive interface** - Well-organized panels
✓ **Lightweight** - No external dependencies

---

## 🎓 Learn by Creating

### Project 1: Simple Baseboard

1. Create a cube (Shift+A > Mesh > Cube)
2. Enter Edit Mode (Tab)
3. Select the bottom face
4. Create a baseboard
5. Adjust height and profile

### Project 2: Room with Frames

1. Model a simple room
2. Add baseboard around
3. Create a door frame
4. Create a window frame
5. Export as FBX/GLTF

---

## 🚀 Best Practices

### Before Generation

✓ Verify your geometry is correct
✓ Check normal orientation
✓ Clean up duplicate faces

### After Generation

✓ Test parameters
✓ Use "Rebuild" to confirm changes
✓ Export when satisfied with result

### Performance

✓ For large scenes, generate by sections
✓ Use "Merge" to combine baseboards if needed
✓ Export to Cycles for rendering

---

## 📈 Roadmap / Future Improvements

Possible improvements:
- [ ] Return of Unwrap and Material panels (optional)
- [ ] More predefined profiles
- [ ] Support for custom profile curves
- [ ] Batch generation for multiple objects
- [ ] Direct export to different formats

---

## 📄 Technical Information

### Required Versions

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| Blender | 5.2.0 | 5.2+ |
| Python | 3.10 | 3.11+ |
| System | Windows/Mac/Linux | All |

### Included Files

```
plinthes_byfred_final/
├── __init__.py              Main code (~84 KB)
└── blender_manifest.toml    Blender manifest
```

### Dependencies

- `bpy` (Blender Python API)
- `bmesh` (Blender Mesh Python API)
- `mathutils` (Blender math utilities)

*All included with Blender - no external installation required*

---

## 💡 Helpful Tips

### Optimize Workflow

1. **Create a preset** for your favorite parameters
2. **Duplicate baseboards** rather than regenerate
3. **Group objects** for better control
4. **Name clearly** your baseboards and frames

### Manage Complexity

- Generate baseboards **last** (after architecture)
- Use **collections** to organize
- **Hide** source objects after generation

---

## ✅ Getting Started Checklist

- [ ] Download plinthes_byfred_modified.zip
- [ ] Extract the folder
- [ ] Copy to Blender addons folder
- [ ] Restart Blender
- [ ] Enable addon in Preferences
- [ ] Open plinthes fred panel (View3D Sidebar)
- [ ] Create your first baseboard
- [ ] Test the parameters

✅ **You're ready to create professional baseboards!**

---

## 🎉 Conclusion

**Plinthes Fred** is a powerful and easy-to-use tool for generating baseboards, door frames, and window frames in Blender.

With this modified version, you have access to **all generation power** in a **simplified and intuitive interface**.

**Happy 3D creation!** 🚀

---

## 📞 Information

- **Original Addon**: byfred
- **Version**: 1.11.0 (Modified)
- **Blender**: 5.2+
- **License**: GPL v3
- **Date**: August 2024

---

**Plinthes Fred - Molding Generator for Blender**

*Transform your 3D architecture in just a few clicks!* ✨
