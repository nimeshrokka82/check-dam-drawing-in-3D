# 3D Check Dam Design – CAD

A step-by-step implementation of a **check dam design workflow** from 2D drafting to 3D modeling. This project documents the process of creating a water-retention structure with proper hydraulic considerations, dimensioning, and 3D extrusion techniques.

---

## 📋 Overview

This repository contains the workflow, commands, and structural details for designing a **check dam** in CAD software, starting from unit setup and 2D line drawing through to 3D extrusion and hydraulic feature integration. The design includes walls, gates, spillways, and erosion-protection elements, following engineering best practices for water management structures.

---

## 🛠️ Workflow Summary

### 1. **Unit & Dimension Setup**
- Units: **Meters** (converted from inches)
- Decimal precision: **2 digits**
- Dimension style: Custom line symbols, leaders, text font (Arial, 2pt height)

### 2. **2D Drafting**
- Base line: **9 meters** (using `LINE` command with `F8` constraint)
- Wall offsets: **3.5m, 0.5m (plinth), 1.5m (dead wall), 2.1m (return wall)**
- Gate: **1 meter** width, placed centrally
- Grouping & trimming for clean structure

### 3. **3D Modeling**
- Transition to **3D Modeling workspace**
- Assign varied wall heights: **1.2m, 1.5m, 2.7m, 2.0m**
- Adjust **UCS** for proper extrusion base
- Extrude 2D profiles to create 3D dam body

### 4. **Hydraulic Features**
- **Sloped overflow** surface
- **Duckbill-shaped spillway** for gentle water release
- **Stone-pitched channel bed** to prevent erosion
- **Tank area** to reduce water velocity & absorb energy

---

## 📐 Structural Dimensions Summary

| Element            | Dimension      | Command Used       | Purpose                     |
|--------------------|---------------|-------------------|-----------------------------|
| Base length        | 9 meters      | `LINE` + `F8`     | Main structure length       |
| Wall thickness     | 3.5 meters    | `OFFSET`          | Parallel walls              |
| Plinth thickness   | 0.5 meters    | `OFFSET`          | Base support layer          |
| Dead wall          | 1.5 meters    | `OFFSET`          | Side reinforcement          |
| Return wall        | 2.1 meters    | `OFFSET`          | Wall return section         |
| Gate width         | 1 meter       | `OFFSET` (removed)| Water flow control          |
| Barrier length     | 4 meters      | `OFFSET`          | Gate-side reinforcement     |
| Wall heights       | 1.2m–2.7m     | 3D extrusion      | Vertical dam components     |

---

## 🔑 Key CAD Commands & Concepts

| Concept / Command       | Purpose                                      |
|-------------------------|----------------------------------------------|
| `UNITS`                 | Set drawing units to meters with 2 decimals  |
| `DIMSTYLE`              | Customize dimension text, lines, and symbols |
| `LINE` (`L`)            | Draw straight lines (use `F8` for ortho)     |
| `OFFSET` (`O`)          | Create parallel lines at specified distances |
| `TRIM` (`TR`)           | Remove unwanted line segments                |
| `EXTEND` (`EX`)         | Lengthen lines to meet boundaries            |
| Group creation          | Organize lines into logical segments         |
| UCS adjustment          | Align coordinate system for 3D extrusion     |
| Extrude                 | Convert 2D shapes to 3D with height values   |

---

## 🏗️ Design Features

### ✅ **Structural Components**
- Concrete walls with varied thickness
- Reinforced plinth base
- Gate opening for controlled flow
- Return walls for structural integrity

### ✅ **Hydraulic Design**
- Sloped overflow to guide water
- Duckbill spillway to reduce water force
- Energy-dissipation tank
- Stone pitching to prevent bed erosion

### ✅ **3D Modeling Approach**
- Parametric height assignment
- Layer-based organization
- Realistic volumetric representation

---
