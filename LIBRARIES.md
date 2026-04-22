# OpenSCAD Library Installation

This guide explains how to install the libraries required to use the skills in this repository.

> **Note:** This document was generated with the assistance of AI.

## Required Libraries

1.  **BOSL2 (The Belfry OpenSCAD Library v2)**: Essential for intent-based modeling and attachments.
2.  **The Boardgame Insert Toolkit (BIT)**: Necessary for creating board game organizers.

## Installation Steps

### 1. Locate your OpenSCAD libraries folder

Open OpenSCAD and go to **File -> Show Library Folder...**. This will open the file explorer in the correct folder for your operating system.

- **Windows:** Usually `Documents\OpenSCAD\libraries`
- **macOS/Linux:** Usually `~/OpenSCAD/libraries`

### 2. Install BOSL2

1.  Visit the repository: [https://github.com/BelfrySCAD/BOSL2/](https://github.com/BelfrySCAD/BOSL2/)
2.  Download the ZIP or clone the repository directly into your `libraries` folder:
    ```bash
    cd [YOUR_LIBRARIES_FOLDER]
    git clone https://github.com/BelfrySCAD/BOSL2.git
    ```
3.  Ensure the folder is named exactly `BOSL2`.

### 3. Install The Boardgame Insert Toolkit (BIT)

1.  Visit the repository: [https://github.com/dppdppd/The-Boardgame-Insert-Toolkit](https://github.com/dppdppd/The-Boardgame-Insert-Toolkit)
2.  Download the files and place the toolkit folder inside your `libraries` folder.
3.  Rename the folder to `BoardgameInsertToolkit` to ensure compatibility with standard paths.

## Verification

After installing, you can verify that OpenSCAD recognizes the libraries by creating a new file and testing the following commands:

```openscad
include <BOSL2/std.scad>
include <BoardgameInsertToolkit/BoardgameInsertToolkit.scad>

// If no "File not found" errors occur, the installation was successful!
cuboid([10,10,10]); // Test BOSL2
```
