# DisplayShift

**Switch between supported monitor inputs directly from Windows.**

DisplayShift is a Windows utility for setups where multiple video outputs connect to the same monitor. Switch between compatible HDMI and DisplayPort inputs, preview another Windows desktop, and access everyday controls in one straightforward interface.

**Latest version:** v1.0.2 · **Publisher:** Zatima · **Platform:** Windows 11 (64-bit) tested · **License:** Proprietary

![DisplayShift v1.0.2 main window](assets/DisplayShift_Main_UI.png)

## Download

Get the latest version from the **[DisplayShift v1.0.2 release page](https://github.com/zatimamo/DisplayShift/releases/tag/v1.0.2)**.

| Version | Download | Details |
| --- | --- | --- |
| **Installer** | [Download for Windows (.exe)](https://github.com/zatimamo/DisplayShift/releases/download/v1.0.2/DisplayShift_V1.0.2_Setup.exe) | Guided installation, Start menu shortcut, optional desktop shortcut, and uninstaller |
| **Portable** | [Download portable (.zip)](https://github.com/zatimamo/DisplayShift/releases/download/v1.0.2/DisplayShift_V1.0.2_Portable.zip) | Extract and run without installing |

Both editions include the application and required runtime files. A separate Python installation is not needed.

You can check download integrity with [SHA-256 checksums](SHA256SUMS.txt).

## Features

- **Monitor input switching:** Select compatible HDMI or DisplayPort inputs through DDC/CI.
- **Keyboard shortcut:** Use **Page Up (Bild ↑)** to switch inputs quickly.
- **Clear display status:** See which input is active, pending, unavailable, or not yet confirmed.
- **Second-desktop preview:** Keep an eye on another Windows desktop with a lightweight 1 FPS thumbnail.
- **Interactive preview:** Open a larger view and optionally control the other desktop with mouse and keyboard.
- **Gaming Mode:** A simpler layout designed to keep background preview and polling activity low.
- **Multiple languages:** English, French, German, Simplified Chinese, and Arabic (right-to-left).

### Input controls

![DisplayShift input selection cards](assets/DisplayShift_Input_Controls.png)

## Getting started

**Installer**

1. Download and run `DisplayShift_V1.0.2_Setup.exe`.
2. Follow the setup wizard.
3. Launch DisplayShift from the Start menu or desktop shortcut.

**Portable**

1. Download `DisplayShift_V1.0.2_Portable.zip`.
2. Extract the entire archive.
3. Open the `DisplayShift_Portable` folder and run `DisplayShift.exe`. Keep the accompanying `_internal` folder in place.

See the [installation guide](INSTALLATION_GUIDE.md) for configuration and troubleshooting.

## Compatibility

DisplayShift relies on **DDC/CI input switching (VCP code 0x60)**. Support varies by monitor, firmware, connection, and input configuration. A monitor may acknowledge a command without completing the physical input switch.

The current version was tested on **Windows 11 (64-bit)** with a **Samsung Odyssey G7** connected to two GPU outputs:

- **HDMI:** NVIDIA GeForce RTX 4070 Ti SUPER
- **DisplayPort:** NVIDIA GeForce RTX 4070

Other Windows 10/11 (64-bit) systems and monitor combinations have not been fully validated. For desktop preview to work, Windows must continue to detect both video outputs. Keep the monitor's physical input controls available if you need to switch back manually.

## What's new in v1.0.2?

This update improves how DisplayShift handles language preferences after installation or upgrades:

- The installer starts in English once after setup, including when upgrading from a saved Arabic-language configuration.
- Your selected language is remembered on later launches.
- Existing display names and input mappings are preserved.
- The portable version keeps previously saved language preferences.

Read the [release notes](RELEASE_NOTES.md) or [changelog](CHANGELOG.md).

## Troubleshooting and support

| Issue | What to check |
| --- | --- |
| **Page Up does not respond** | Another program may be using the shortcut. Check its status in DisplayShift. |
| **Input status stays amber** | Check the monitor's actual picture. Input readback can be ambiguous. |
| **Second-desktop preview is unavailable** | Make sure Windows still detects both video outputs. |
| **Your monitor does not switch** | Confirm DDC/CI is supported and enabled, and that its input codes match your setup. |

For additional help or to report a problem, see [Support](SUPPORT.md).

## Privacy and licensing

DisplayShift uses local Windows APIs for monitor switching and desktop preview. These functions do not require an online account or cloud service. Preferences are stored locally in `%LOCALAPPDATA%\DisplayShift\settings.json`.

**DisplayShift is closed-source software.** The repository contains public documentation, screenshots, and links to compiled downloads. It does **not** contain the application's private source code. GitHub's automatically generated source archives include only the public repository files.

The app is not digitally signed with a trusted Windows code-signing certificate, so Windows may display an unknown-publisher warning.

See the [proprietary license](LICENSE), [third-party notices](THIRD_PARTY_NOTICES.txt), and [security information](SECURITY.md). Licenses for bundled components, including Qt/PySide6, continue to apply.

**Made with love ♥ · Zatima**

© 2026 Zatima. All rights reserved, subject to applicable third-party license terms.
