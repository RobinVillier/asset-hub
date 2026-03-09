# Asset Hub

Asset Hub is a **Maya pipeline tool** designed to organize and manage production assets through a structured project hierarchy.

Asset Hub helps artists and technical directors maintain **consistent file organization, versioning, and asset structure** across multiple clients and projects.

<img width="1778" height="1000" alt="ArtstationPost_001" src="https://github.com/user-attachments/assets/6cb58360-3f12-4573-a851-08834c976513" />

---

## Features

- **Automatic asset organization** using a `Client / Project / Asset / Task` hierarchy.
- **Integrated versioning system** with version-up and publish options.
- **Save As workflow** to ensure consistent file naming.
- **Recent files panel** for quick access to previously opened scenes.
- **Project template hierarchy generator**.
- **Direct access to Maya project folders**.
- Clean and efficient **Qt interface (PySide2 / PyQt)**.
- Designed for **production-friendly Maya pipelines**.

---

## Interface Overview

The tool provides three main interfaces:

### Main Asset Browser

Browse clients, projects, assets, and tasks while viewing all versions of the selected file.

### Save As Window

Allows artists to:
- Version up scenes
- Publish files
- Automatically generate proper filenames

### Settings Panel

Configure:
- Project root path
- Default task
- Recent file limits
- Template hierarchy structure

---

## Project Structure


AssetHub/\n
├── config/ # Tool configuration and settings\n
├── core/ # Core pipeline and asset management logic\n
├── ui/ # Qt-based user interface\n
├── wdigets/ # Qt-based custom widgets\n
└── resources/ # Icons, stylesheets, and UI assets\n


---

## Installation

1. Copy the **AssetHub** folder into your Maya scripts directory.

Typical locations:

### Windows


Documents/maya/scripts


### Linux / Mac


~/maya/scripts


2. Restart Maya or reload the Python path.

---

## Usage

Launch the tool from Maya's Script Editor or a shelf button.

```python
from BetterFileExplorer import main
main.launch_app()
```

Files will automatically follow the correct naming and versioning conventions.

Example File Hierarchy :

ProjectRoot/\n
└── Client\n
    └── Project\n
        └── Assets\n
            └── AssetName\n
                └── rig\n
                    ├── AssetName_rig_v001.001.ma\n
                    ├── AssetName_rig_v001.002.ma\n
                    ├── AssetName_rig_v002_pub.ma\n
                    ├── AssetName_rig_v002_001.ma\n
                    ├── AssetName_rig_v002_002.ma\n
                    └── AssetName_rig_v002_003.ma\n

## Contacts
For issues, questions, or contributions:
Email: rvillier99@gmail.com
