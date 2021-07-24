- [1. User interface](#1-user-interface)
  - [1.1 3d viewport](#11-3d-viewport)
  - [1.2 Tool Bar](#12-tool-bar)
- [2. Modelling](#2-modelling)
  - [Overall](#overall)
  - [2.1 Edit Mode](#21-edit-mode)
    - [2.1.1 Selecting](#211-selecting)
  - [2.2 [Modifier Properities]](#22-modifier-properities)
  - [2.3 Particle](#23-particle)
- [3. Sculpting](#3-sculpting)
  - [Overall](#overall-1)
- [4. Materials](#4-materials)
- [5. Lighting](#5-lighting)
- [6. Rendering](#6-rendering)
  - [Overall](#overall-2)
  - [6.1 Camera](#61-camera)
- [7. Shading](#7-shading)
- [8. Texture Paint](#8-texture-paint)
  - [8.1 Procedure Texture](#81-procedure-texture)
---

# 1. User interface

## 1.1 3d viewport

**Overall**

|View Action|shortcut|
|---|---|
|Orbiting| Mouse Mid |
|Pan| Shift + Mouse Mid|

> **gizmo** if no Mouse or Mid button, can use gizmo on Up-Right corner to Orbiting or Pan or Zoom etc.

> `Shift + Space` Toggle Toolbar, Gives more Shortcut hint.

|Action|shortcut|
|---|---|
|Move 3D Cursor| Shift + MouseR|
|Center 3D Cursor| Shift + C|

|Window Action|shortcut|
|---|---|
|Toggle Properities Sidebar|n|
|Splitting View| MouseR on Window-border / MouseL Drag Corner|
|Merge Splitted View| MouseR on Window-border to Join / MouseL Drag corner|
|Maximum current window| Ctrl + Space |
|Switch Mode| Ctrl + Tab|

|View Action|shortcut|
|---|---|
|Fucus | ~ |

## 1.2 Tool Bar

> Move, Rotate, Scale

**Overall**

`Mouse R` to cancel while hold `Mouse L`

`BTN` + `x/y/z` Constraint x or y or z

`BTN` + `Mouse Mid` Auto Constraint.

| Basic Action | Shortcut |
| --- | ---- |
| Grab | G |
| Rotate | R |
| Scale | S |

---


# 2. Modelling

## Overall

`Shift a` Add

`[Sence Properties] - [Units]` Change Unit

`Select Object` + `Mouse R` change **Shade Smooth** or **Shade Flat** in Normal viewport

Change the preset view (4 methods)
- [Numpad] or 
- Click `gimzo` or
- `~` or
- `[alt]` + `<Mouse Mid Drag>`

`Toggle [X-Ray]`  Can select point that was hide in.

`Shift D` Duplicate

`h` Hiding  
`alt h` not hiding

`m` Move to Collection.

| Basic Action | Shortcut |
| --- | ---- |
| Set Parent | Ctrl + P |



## 2.1 Edit Mode

`Tab` Enter Edit mode

`O` Proportional Editing  
- `Scroll Up` Proportional size down  
- `Scroll Down` Proportional size up

`p` Seperate

`[Snap Tool]` to snap

Select 2 vertices `e`  : extrude.

### 2.1.1 Selecting

`Ctrl` + `L` Select all connected to selected-Vertices.

`a` Select all mesh  
`alt + a`  DeSelect

`alt` + `Mouse L` Click line to select the loop.

`Ctrl i`  Invert Select  ( [Select] - [Invert] )


select Mesh `mouse R - [Subdivide]` Mesh Level add subdivide

## 2.2 [Modifier Properities]

> Modifier item works in order, from up to down.

> Make a backup geometry before Apply a Modifier, apply cannot go back.

> ApplyModifier Properityes in Normal-Viewport

Add `[Subdivision Surface]` in the drop list

Add `[Solidify]`  give extrude, thickness

## 2.3 Particle

> Weight Paint Mode (After Draw Will Create a Vertex Group, Can be used to Particle Density)

> Set Object Origin.  (object, MouseR -> Set Origin)


---
# 3. Sculpting

## Overall

| Action | ShortCut |
|---|---|
| Brush Size | F |
| Brush Strenth| Shift F|
| Push | hold Ctrl|

---

# 4. Materials

---
# 5. Lighting

---
# 6. Rendering

## Overall

|Action| ShortCut|
|---|---|
|Switch Render Mode in Viewport| Z |
|Bring up the most recent render| F11 |

> Render Engine:  Eevee VS Cycles


## 6.1 Camera

> Basic color, Roughness, Subsurface，Light, Denoise, Compositing

> Camera is View of Render, Could Lock Camera to View

|Camera Action| ShortCut|
|---|---|
| Camera View |  Numpad 0 |
| Move Camera to current View | Ctrl + Alt + Numpad 0 |

# 7. Shading

> Using Node view

|Shading Node used|Properity|Output|
|---|---|---|
|Object Info|Random|output random Num from 0 to 1|
|ColorRamp||Map 0..1 to ColorRamp |

# 8. Texture Paint

Create new image in [Texture Paint Workspace]
Add 'image texture' node in [Shading Workspace], and add image to this node.

> Using Texture Mask to change brush type
> - Add new Texture in [Texture Properities]
> - Change Masking Mapping in  from [Tiled] to [random] to looks Smooth.

## 8.1 Procedure Texture

> Turn Add-on `Node Wrangler` in Blender Preferences. THen I can use shortcut `Ctrl  + Shift + MouseL` To Quick Preview the Node in the final.

> Fake Bump or Real Bump ('rough and uneven in surface' is looks like or Real affect the Mesh)
> - [ Material Properities ] - [ Settings ] - [ Displacement ] - [ Displacement and Bump ]