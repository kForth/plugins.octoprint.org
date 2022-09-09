---
layout: plugin

id: poweroffafterprint
title: OctoPrint-PowerOffAfterPrint
description: TODO
authors:
- Kestin Goforth
license: AGPLv3

date: 2022-09-09

homepage: https://github.com/kforth/OctoPrint-PowerOffAfterPrint
source: https://github.com/kforth/OctoPrint-PowerOffAfterPrint
archive: https://github.com/kforth/OctoPrint-PowerOffAfterPrint/archive/main.zip

tags:
- auto off
- auto_shutdown
- control
- power

screenshots:
- url: /assets/img/poweroffafterprint/sidebar_enabled.png
  alt: Sidebar Screenshot - Enabled
  caption: Quickly Enable/Disable the plugin
- url: /assets/img/poweroffafterprint/sidebar_disabled.png
  alt: Sidebar Screenshot - Disabled
  caption: Quickly Enable/Disable the plugin
- url: /assets/img/poweroffafterprint/settings.png
  alt: Settings Screenshot
  caption: Plugin Settings

featuredimage: /assets/img/poweroffafterprint/sidebar.png

compatibility:

  octoprint:
  - 1.4.0

  python: ">=3,<4"

---


# OctoPrint-PowerOffAfterPrint

Automatically shutdown your 3D Printer after a print is done.

## Setup

Install via the bundled [Plugin Manager](https://docs.octoprint.org/en/master/bundledplugins/pluginmanager.html)
or manually using this URL:

`https://github.com/kforth/OctoPrint-PowerOffAfterPrint/archive/main.zip`

## Configuration

After installation, open OctoPrint settings (wrench icon) and scroll down to the "PowerOffAfterPrint Plugin" page.

You can configure the following options:

| Option | Default | Description |
|:-------|:--------|:------------|
|`Power Off Script`| M81 | The commands sent to the printer to shutdown. |
|`Power Off On Done`| True | Power off the printer if the print was successful. |
|`Power Off On Fail`| True | Power off the printer if the print failed. |
|`State On Startup`| Unchanged | Initial state for plugin when OctoPrint starts. |
|`State On Print Start`| Disabled | Automatically set the current state when a print is started. |
|`State On Print End`| Disabled | Automatically set the current state when a print is finished. |
