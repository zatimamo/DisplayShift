# DisplayShift Official V1.0.2
**Publisher: Zatima** | **Made with love ♥**

## Short app description
DisplayShift is a lightweight Windows monitor-input controller that makes it easier to switch between compatible HDMI and DisplayPort connections. It also lets you preview and interact with another Windows desktop without using the monitor's physical input button.

## Detailed description
Designed for Windows setups with multiple GPU outputs connected to one monitor, DisplayShift uses DDC/CI commands to request an input change. Its clean dashboard features named display cards, clear input status indicators, keyboard shortcuts and an optional preview of a different Windows desktop.

Use the small 1 FPS thumbnail to see the other desktop, expand it for interactive mouse/keyboard control, or use Gaming Mode for a simpler, reduced-activity interface.

## Main features
- Switch supported monitor inputs using DDC/CI VCP 0x60
- Page Up / Bild ↑ global switching hotkey
- Renameable input cards and active/pending/error status
- 1 FPS second-screen thumbnail
- Interactive expanded desktop preview and window-moving controls
- Gaming Mode with simpler controls
- English, French, German, Simplified Chinese and Arabic (RTL) user interface
- Teal dual-arrow icon and two-line publisher credit

## Compatibility
Tested around a Samsung Odyssey G7 with an HDMI GPU output and a separate DisplayPort GPU output. Compatibility is monitor- and connection-dependent: not all monitors support the required DDC/CI commands. A successful DDC write does not always prove that the picture switched. Windows must detect both outputs for preview to work.

Windows 11 x64 has been tested. Other Windows 10/11 x64 environments are not comprehensively validated.

## Language
Installer: English on the first launch after installing or upgrading. Later preferences are remembered.
Portable: English on a fresh profile; existing profiles retain their saved language.

## Distribution
DisplayShift's own application code is proprietary and closed-source. The public packages contain compiled binaries rather than editable source. Bundled third-party components, including Qt/PySide6, retain their separate licenses and user rights.

Copyright © 2026 Zatima. All rights reserved.
