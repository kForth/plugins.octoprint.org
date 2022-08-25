---
layout: plugin

id: CreatbotUtil
title: Creatbot Util
description: Various utility functions to make OctoPrint work better with Creatbot printers.
author: Kestin Goforth
license: AGPLv3

date: 2022-06-14

homepage: https://github.com/kForth/OctoPrint-CreatbotUtil
source: https://github.com/kForth/OctoPrint-CreatbotUtil
archive: https://github.com/kForth/OctoPrint-CreatbotUtil/archive/main.zip

follow_dependency_links: false

tags:
- creabot
- printer
- control
- command
- serial
- start
- stop
- temperature
- heated
- chamber
- build
- volume

# featuredimage: null

screenshots:
- url: /assets/img/plugins/CreatbotUtil/controls.png
  alt: Control Tab Screenshot
- url: /assets/img/plugins/CreatbotUtil/settings.png
  alt: Settings Page Screenshot

compatibility:
  python: ">=2.7,<4"

---

## Features

- Send "Start/Stop Serial Print" commands whenever a print is started, cancelled, or finished (M6006 & M6007).
  - Optionally send "Start/Stop" commands whenever a print is paused or resumed.
- Replace the Marlin 'Set Chamber Temperature' command (M141) with the CreatBot command (M6013).
- Adds `Extruder Auto Fan` and `Chamber Air Fan` controls to the Control Tab
- Adjust you printer's `Time Used` and `Registered Time` values.
- Enable plugin for all or only selected printer profiles.

  *See the plugin's [homepage](https://github.com/kForth/OctoPrint-CreatbotUtil) for most up to date list of features.*

## Setup

Install the latest release via the bundled [Plugin Manager](https://docs.octoprint.org/en/master/bundledplugins/pluginmanager.html) then retart your OctoPrint instance.

## Notes

This plugin should work for most/all CreatBot 3D Printers but has only been tested with a CreatBot F430.

You may need to upgrade your printer's firmware to take full advantage of this plugin's features.
The original v5.5 firmware that shipped with my CreatBot F430 did not support the Heated Chamber (M6013) command, an upgrade to v5.6 was required.
