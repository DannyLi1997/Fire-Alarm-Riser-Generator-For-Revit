# Fire Alarm Riser Generator For Revit

A Revit add-in that draws fire alarm riser diagrams for you, straight from the devices on your floor plans.

> Showcase repository. The source code is private.

## Why
On a high-rise project, the riser diagram can take days to draw by hand, and it has to match the floor plans device for device. Fire Alarm Riser Generator reads the devices, addresses, and circuits already in the model and lays out the riser in minutes.

## Features
- Reads device addresses, panels, and circuits from floor plan views
- Draws SLC devices in floor plan wiring order
- Handles strobe, speaker, and combined notification circuits, each with its own home run to the control panel
- Keeps wire labels and colors consistent per run and creates missing line styles automatically
- Places end-of-line (EOL) resistors and standard circuit notes
- Draws stair risers as separate columns for stair speakers, smoke detectors, and sprinkler modules
- Shows panels, power supplies, and surge suppressors with their modules
- Manufacturer presets for Autocall and Gamewell-FCI, plus a custom mode
- Tabbed settings window and a code-signed build
- Supports Revit 2019 through 2025+

## Built with
C# · .NET · Revit API · Windows Forms · Visual Studio

## Screenshots
<!-- Example: ![Generated riser](screenshots/riser.png) -->
### 1. Devices
Pick which view to scan and which device categories to include. Each device type is matched to its riser symbol and tag automatically from family names, and any row can be overridden by hand.

<img width="1182" height="852" alt="image" src="https://github.com/user-attachments/assets/148f6aa5-3bf2-4a35-87aa-77fac023d5da" />

### 2. Addressing
Choose the fire alarm manufacturer and the preset fills in address, panel, and wire label rules. Fine-tune how addresses are read, show devices that sit on two circuits (such as a speaker strobe on both its strobe and speaker circuit), place EOL resistors, and include devices that don't have an address yet.

<img width="1182" height="887" alt="image" src="https://github.com/user-attachments/assets/e42f65a2-ddc4-45dc-8355-2257d8ac9fe7" />

### 3. Output & Tags
Set the drafting view name, scale, text and line styles, and where the view lands in the project browser. Tags can learn their positions from ones you adjusted by hand in the last riser, and wire labels are assigned per circuit type.

<img width="1182" height="887" alt="image" src="https://github.com/user-attachments/assets/175045b1-0c82-4bad-9cf7-7c1ad0f97078" />

### 4. Layout
Control real drafting dimensions such as device spacing, row spacing, and devices per row, plus layout rules: one FACP per floor, separate sprinkler and stair risers, surge suppressors under amplifier and power panels, and module groups boxed as they appear on the plan.

<img width="1182" height="887" alt="image" src="https://github.com/user-attachments/assets/1531db5e-5b0e-47c4-9f1d-2fec189dd774" />

### 5. Generated riser
One floor's electrical room as generated: wire trough, amplifier, power, and module panels with surge suppressors and power notes, the SLC loop on the left, and speaker and strobe circuits on the right with wire labels, colors, EOL resistors, and circuit notes placed automatically.

<img width="3255" height="1026" alt="Screenshot 2026-10-21 181538" src="https://github.com/user-attachments/assets/f6024508-c9f9-4527-8d4f-b91c732fcb98" />

