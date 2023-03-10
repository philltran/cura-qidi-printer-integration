# Cura-QidiPrint Plugin

## Plugin for Cura 5.2 that allows monitoring and printing Qidi 3D printers over network 

![Screenshot of the print button](./screenshots/print-button.png)

![Screenshot of the monitor stage](./screenshots/monitor.png)

## Installation via Cura Marketplace

Simply open Cura and go to the **Marketplace** in the menubar, search for the QidiPrint plugin and install it!

## Manual Installation

With Cura not running, unpack the zip file from the
[release](https://github.com/philltran/cura-qidi-printer-integration/releases) to this
specific folder:

  * Windows: `%USERPROFILE%\AppData\Roaming\cura\5.2\plugins\`
  * MacOS: `~/Library/Application Support/Cura/5.2/plugins/`
  * Linux: `/home/<username>/.local/share/cura/5.2/plugins/`

If you don't have Qidi printers available in Cura, unpack the [Qidi Printer Definitions.zip](https://github.com/philltran/Cura-Qidi-Printer-Definitions/archive/refs/tags/v5.2.1.zip) to this specific folder:
  * Windows: `%USERPROFILE%\AppData\Roaming\cura\5.2\`
  * MacOS: `~/Library/Application Support/Cura/5.2/`
  * Linux: `/home/<username>/.local/share/cura/5.2/`

## Configuration

**Do NOT try to add a new "networked printer"!** This is only for Ultimaker printers.

**If you did not use printer definitions archive from above to add Qidi printer, in order for this plugin working properly, your printer.def.json must have "manufacturer" property set to "Qidi"**

QIDI printers are configured through the extension menu bar:

* Start Cura
* Inside the cura Prefernces->Printers selct and activate your printer
* Click "QidiPrint" button right to the Machine Settings button:

![Screenshot of the menu bar entry](./screenshots/menu-bar.png)

* A new window will pop-up with detected printers list (you also can add them manually by pressing the Add button)

![Screenshot of the discovery dialog](./screenshots/discovery-window.png)

* Choose your printer and press the "Connect" button
* Click "Close"
* Done!

Now you can load a model and slice it. Then look at the bottom right - there
should be the big blue button with you printer name on it!

## License

Thank you to Nick Kuvyrkin ([nkuvyrkin](https://github.com/nkuvyrkin)), [ducphuc](https://github.com/ducphuc), [jvrobert](https://github.com/jvrobert) and [alkaes](https://github.com/alkaes) for working on Cura 5.x support.

This project is inspired and using code from:
* https://github.com/Kriechi/Cura-DuetRRFPlugin
* https://github.com/Jeredian/mks-wifi-plugin
* https://github.com/alkaes/QidiPrint
* ChituCodeWriter.py is taken from https://github.com/Spanni26/ChituCodeWriter
