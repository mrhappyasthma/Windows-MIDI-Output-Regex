# Windows-MIDI-Output-Regex
A regex for Windows 7/10 to default MIDI files to output to USB. This is useful for my player piano.

If the PC is playing the track instead of outputting it to MIDI, you need to update the default MIDI
output device in the registry.

This file edits the following path:

```
HKEY_CURRENT_USER\Software\Microsoft\ActiveMovie\devenum\{4EFE2452-168A-11D1-BC76-00C04FB9453B}\Default MidiOut Device
```

It sets the `MidiOutId` field to a value of `1`.

Source:
https://answers.microsoft.com/en-us/windows/forum/windows_7-pictures/windows-7-midi-output-device-selection/60b7cb85-b0ca-449b-9b62-0738b8c8585b
