# Installing DisplayShift

Choose the **installer** for a standard Windows setup or the **portable ZIP** if you'd prefer to run DisplayShift without installing it.

## Windows installer

1. [Download DisplayShift v1.0.2 Setup](https://github.com/zatimamo/DisplayShift/releases/download/v1.0.2/DisplayShift_V1.0.2_Setup.exe).
2. Run the downloaded file and follow the setup wizard.
3. Choose whether to create a desktop shortcut.
4. Open DisplayShift from the Start menu or desktop shortcut.

The installer includes an uninstaller. On the first launch after installation or upgrade, DisplayShift starts in English. You can change the interface language in **Preferences**, and your selection will be remembered afterward.

## Portable edition

1. [Download DisplayShift v1.0.2 Portable](https://github.com/zatimamo/DisplayShift/releases/download/v1.0.2/DisplayShift_V1.0.2_Portable.zip).
2. Extract the entire ZIP file.
3. Open the extracted `DisplayShift_Portable` folder.
4. Run `DisplayShift.exe`. Do not separate it from the bundled `_internal` folder.

No installer or separate Python installation is required. The portable edition keeps existing language preferences.

## Preferences

Both editions store preferences under your Windows user profile:

`%LOCALAPPDATA%\DisplayShift\settings.json`

If you use both editions on the same Windows account, they share those preferences. Installing or upgrading does not intentionally reset your display names or input mappings.

## Before switching inputs

Check that your monitor supports **DDC/CI input selection** and that Windows detects the video outputs you want to use. Actual input codes and behavior vary by monitor. Keep the physical input selector available in case switching needs to be done manually.

## Troubleshooting

- **Page Up doesn't respond:** Check the app's hotkey indicator and close any other program using the key.
- **Input status remains amber:** Look at the monitor. The readback may not clearly confirm the physical switch.
- **Preview does not appear:** Verify that Windows detects both outputs.
- **Input switching fails:** Check DDC/CI support, monitor settings, connections, and input codes.

For further assistance, read [Support](SUPPORT.md).

## Windows security warning

DisplayShift is not signed with a trusted Authenticode certificate. Windows may therefore display an unknown-publisher warning. Download only from the [official GitHub Releases page](https://github.com/zatimamo/DisplayShift/releases) and verify the published [checksums](SHA256SUMS.txt).
