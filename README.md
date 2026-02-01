# SpiralGen - KiCad 9 Plugin

**SpiralGen Pro** is an advanced Python plugin for KiCad 9 that automates the generation of planar spiral inductors. It combines geometric algorithms with physics-based inductance estimation.

## Features
- **Multi-Geometry Support**: Circular, Square, and Octagonal spirals.
- **Inductance Calculator**: Real-time estimation (in nH) using Mohan's approximations.
- **Center Via Stitching**: Optional automatic placement of a center via.
- **Parametric Design**: Full control over turns, width, spacing, and radius.

## Installation

1. Locate your KiCad scripting folder. Usually:
   - **Mac**: `~/Documents/KiCad/9.0/scripting/plugins`
   - **Windows**: `%USERPROFILE%\Documents\KiCad\9.0\scripting\plugins`
   - **Linux**: `~/.local/share/kicad/9.0/scripting/plugins` or `~/.kicad/scripting/plugins`

   *Note: If the directory does not exist, create it.*

2. Copy the entire `SpiralGen` folder from this repository into the `plugins` directory.

3. Restart KiCad.

## Usage

1. Open **PCB Editor** in KiCad.
2. Look for the "SpiralGen" icon in the top toolbar (or find it in the "Tools" > "External Plugins" menu).
3. Click to open the dialog.
4. Enter parameters:
   - **Shape**: Select Circular, Square, or Octagonal.
   - **Number of Turns**: E.g., 5.
   - **Track Width/Spacing**: (mm).
   - **Inner Radius**: (mm).
   - **Options**: Check "Add Center Via" if needed.
   *Observe the Estimated Inductance value updating as you change parameters.*
5. Click **OK**.

## Verification
To verify the math logic without KiCad, run the included `verify_math.py`:
```bash
python3 verify_math.py
```
