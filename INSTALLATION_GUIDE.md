# DisplayShift V1.0.2: Installation Guide

## Installer (recommended)
1. Run DisplayShift_V1.0.2_Setup.exe.
2. Follow the Windows installation wizard and select your desired folder.
3. Choose whether to create a Desktop shortcut.
4. Launch DisplayShift from the shortcut or Start menu.
5. The first launch after setup uses English. Select another language under Preferences if preferred.

The installed edition includes an uninstaller.

## Portable edition
1. Extract DisplayShift_V1.0.2_Portable.zip completely.
2. Open the resulting DisplayShift_Portable folder.
3. Run DisplayShift.exe from that folder. Keep the bundled _internal runtime files together with the executable.

No installer or separate Python installation is required.

## Configuration
Both editions save user settings under %LOCALAPPDATA%\DisplayShift\settings.json. Under the same Windows user account, both editions can share the saved configuration. The installer resets only the interface language once after setup; input mapping and display names are preserved.

## Troubleshooting
- Page Up shortcut does not work: check the app's keyboard indicator or possible hotkey conflict.
- Display status is amber: verify the physical monitor picture; a DDC command can have ambiguous readback.
- Preview unavailable: confirm both outputs are detected in Windows.
- Not opening on other hardware: DDC/CI support and input codes vary by monitor.

The binary is not signed with a trusted Authenticode certificate, so Windows might display an unknown publisher warning.
