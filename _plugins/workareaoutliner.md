---
layout: plugin

id: workareaoutliner
title: OctoPrint-WorkAreaOutliner
description: Adds a button to show the working area of a gcode file.
author: Kestin Goforth
license: AGPLv3

date: 2022-07-13

homepage: https://github.com/kforth/OctoPrint-WorkAreaOutliner
source: https://github.com/kforth/OctoPrint-WorkAreaOutliner
archive: https://github.com/kforth/OctoPrint-WorkAreaOutliner/archive/master.zip

follow_dependency_links: false

tags:
- Helper
- Preview

# featuredimage: null

screenshots:
- url: /assets/img/plugins/workareaoutliner/screen.png
  alt: Main screen with Outline button
  caption: Outline button and plugin output
- url: /assets/img/plugins/workareaoutliner/settings.png
  alt: Settings screen
  caption: Settings screen.

compatibility:
  python: ">=3,<4"

---
## Description

## Description
This plugin adds an "Outline WA" button to preview the working area of a Gcode file.

If using a supported slicer program, this plugin can read the work area from the file's metadata.

If there is no bounding box in the gcode metadata or if you're using an unsupported slicer, WorkAreaOutliner will use OctoPrint's gcode interpreter to analyze the file.

### Supported Slicers:
- PrusaSlicer
- SuperSlicer
- Slic3r
- Lightburn (inherited from OctoPrint-Framer, untested)
- Fusion360 (inherited from OctoPrint-Framer, untested)

## Setup
### Installation
Install via the bundled [Plugin Manager](https://docs.octoprint.org/en/master/bundledplugins/pluginmanager.html) or manually using this URL:

    https://github.com/kforth/OctoPrint-WorkAreaOutliner/archive/master.zip

## Usage
### Configuration
After installation, restart OctoPrint and go to the Settings tab to configure the plugin.

### Outline Function
- Connect to the machine
- Home the machine (or set origin manually)
- Load the Gcode file
- Navigate to the 'Control' tab and click the 'Outline WA' button
- Watch the machine as it outlines the bounding box of the work area
  - Be ready to stop the machine to avoid colisions!

## License

Copyright © 2022 [Kestin Goforth](https://github.com/kforth/).

Based on work from [Ricardo Riet Correa](https://github.com/rriet/OctoPrint-Framer).

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) for more details.