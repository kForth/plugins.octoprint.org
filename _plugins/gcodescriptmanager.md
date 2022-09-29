---
layout: plugin

id: gcodescriptmanager
title: OctoPrint-GcodeScriptManager
description: Easily manage multiple GCODE scripts.
authors:
- Kestin Goforth
license: AGPLv3

date: 2022-09-29

homepage: https://github.com/kforth/OctoPrint-GcodeScriptManager
source: https://github.com/kforth/OctoPrint-GcodeScriptManager
archive: https://github.com/kforth/OctoPrint-GcodeScriptManager/archive/main.zip

tags:
- gcode
- scripts

screenshots:
- url: /assets/img/gcodescriptmanager/sidebar.png
  alt: Sidebar Screenshot
  caption: Screenshot of the sidebar manager.
- url: /assets/img/gcodescriptmanager/tab.png
  alt: Tab Screenshot
  caption: Screenshot of the plugin tab.
- url: /assets/img/gcodescriptmanager/editdialog.png
  alt: Edit Dialog Screenshot
  caption: Screenshot of the edit dialog.

featuredimage: /assets/img/gcodescriptmanager/sidebar.png

compatibility:
  python: ">=3,<4"

---

# OctoPrint-GcodeScriptManager

Easily manage multiple GCODE scripts.

## Features:

- Multiple GCODE Scripts for each script type
- Add scripts to the sidebar for easy access
- Enable/Disable each script individually

## Setup

Install via the bundled [Plugin Manager](https://docs.octoprint.org/en/master/bundledplugins/pluginmanager.html)
or manually using this URL:

    https://github.com/kforth/OctoPrint-GcodeScriptManager/archive/main.zip

## Configuration

GCODE Script Settings:

- **Name**
  - Easily identifieable name for script.
- **Type**
  - The type of GCODE script.
    - `afterPrinterConnected`
    - `beforePrinterDisconnected`
    - `beforePrintStarted`
    - `afterPrintCancelled`
    - `afterPrintDone`
    - `beforePrintPaused`
    - `afterPrintResumed`
    - `beforeToolChange`
    - `afterToolChange`
- **When**
  - When to execute the script, relative to the default GCODE script of the same type.
    - `Before Default Script`
    - `After Default Script`
- **Script**
  - The GCODE command(s) to execute.
- **Enabled**
  - If `true`, the script will be executed with the default GCODE script of the same type.
    - `true` / `false`
- **SidebarToggle**
  - If `true`, the script will be added to the sidebar manager.
    - `true` / `false`
