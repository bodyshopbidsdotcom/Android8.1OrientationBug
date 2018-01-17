# Android8.1OrientationBug

This repository serves as an example of a bug found in Android 8.1.0

All it has are two Activities:
- `MainActivity` - The manifest restricts it to Portrait orientation
- `Main2Activity` - The manifest has NO restriction on orientation, so you can flip to landscape if you'd like

Issue behavior and steps to reproduce:
1. User starts app and enters MainActivity
2. User presses button to start Main2Activity and enters it
3. User clicks the hardware back button
4. User re-enters MainActivity
5. User turns the phone 90 degrees (either way) and MainActivity orients to Landscape for less than a second, then flips back to Portrait

## Devices reproduced on so far ##

Pixel 2 on Android 8.1.0
