# MUSTBE Panel for Autodesk Revit

Custom ribbon panel for architectural documentation workflows — batch exports, auto-sections, assembly generation, and sheet management.

![Revit](https://img.shields.io/badge/Revit-2022--2025-blue?style=flat-square)
![Language](https://img.shields.io/badge/C%23-.NET-informational?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

---

## What's in it

### Schedules
- **Fix Schedules** — corrects formatting issues that appear when schedules are exported or transferred between models

### Tools
- **Category Sets** — manages shared parameter category sets across the project
- **DXF Batch** — batch-exports selected views or sheets to DXF format

### Doors and windows
- **Door Sections** — generates section views through selected door families automatically
- **Curtain Wall Sections** — cuts sections at panel boundaries for curtain wall elements

### Views
- **Clone Sheets** — duplicates sheets with title block and view placement intact
- **Flush Views** — aligns crop regions across selected views to a common boundary
- **Export to PDF** — exports sheets to PDF using current print settings without opening the print dialog

### Assemblies
- **Assemblies + Views** — creates assemblies from selected elements and generates the standard view set in one step
- **Assembly Sheets** — places assembly views onto a sheet using the project's title block template

---

## Why I built this

Repetitive workflows in architectural documentation — generating sections, exporting sheets, setting up assemblies — eat a disproportionate amount of time on production projects. Each tool in this panel was written to solve a specific bottleneck I ran into repeatedly on real projects.

The panel is grouped by task (what am I doing right now) rather than by Revit's default object categories.

---

## Installation

1. Clone or download this repository
2. Build the solution in Visual Studio (`Release` configuration)
3. Copy the compiled `.dll` and the `.addin` manifest to:
   %APPDATA%\Autodesk\Revit\Addins[Revit version]\
4. Restart Revit — the **MUSTBE** tab appears in the ribbon

---

## Tech stack

- **Platform:** Autodesk Revit 2022–2025
- **Language:** C# (.NET Framework)
- **API:** Revit API
- **Deployment:** `.addin` manifest + ribbon registration on startup

---

## License

MIT
