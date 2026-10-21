# Fire Alarm Riser Tool For Revit

A Revit add-in that draws fire alarm riser diagrams for you, straight from the devices on your floor plans.

> Showcase repository. The source code is private.

## Why
On a high-rise project, the riser diagram can take days to draw by hand, and it has to match the floor plans device for device. FireAlarmRiser reads the devices, addresses, and circuits already in the model and lays out the riser in minutes.

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
<img width="1182" height="852" alt="image" src="https://github.com/user-attachments/assets/148f6aa5-3bf2-4a35-87aa-77fac023d5da" />
