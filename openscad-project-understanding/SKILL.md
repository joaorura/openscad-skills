---
name: openscad-project-understanding
description: Use when Gemini CLI needs to structure, organize, or manage a complex OpenSCAD project.
---

# OpenSCAD Project Understanding

> **Note:** This content was generated with the assistance of AI.

## Overview
Guidelines for organizing OpenSCAD projects for long-term maintainability, focusing on modularity and clear parameter management.

## Project Structure (Recommended)
Follow this file organization for complex models:
- **main.scad**: Primary assembly file (contains `include` and `use` calls).
- **params.scad**: Global parameters and design constants.
- **modules/**: Directory for individual component modules.
- **libraries/**: Directory for external libraries (BOSL2, BIT) if not in standard library paths.

## Modularity: `include` vs `use`
- **`include <file.scad>`**: Imports all variables, constants, and executes top-level code. Use for parameters and global constants.
- **`use <file.scad>`**: Imports modules and functions without executing top-level code or importing variables. Use for component files.

## Library Integration
- **BOSL2**: Always check for `include <BOSL2/std.scad>` at the top of the project.
- **BIT**: Use `include <BoardgameInsertToolkit/BoardgameInsertToolkit.scad>`.

## Best Practices
1. **Parametric First**: Never hardcode dimensions; use variables defined in a central location.
2. **Naming Conventions**: Use `SNAKE_CASE` for global constants and `camelCase` for local variables.
3. **Documentation**: Every module should have a comment describing its purpose and arguments.



