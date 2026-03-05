---
name: say
description: This skill should be used when the user asks to "say" something out loud, e.g. "say hello", "say all done", "say the task is complete". Speaks the message through the system speakers using Windows TTS.
version: 1.0.0
---

# Say (Windows TTS)

When the user asks you to "say" something, speak it aloud using Windows built-in text-to-speech.

## How to use

Run the following PowerShell command, replacing the message text:

```bash
powershell -c "Add-Type -AssemblyName System.Speech; (New-Object System.Speech.Synthesis.SpeechSynthesizer).Speak('your message here')"
```

## Example

User: "say all done"

Run:
```bash
powershell -c "Add-Type -AssemblyName System.Speech; (New-Object System.Speech.Synthesis.SpeechSynthesizer).Speak('all done')"
```

## Notes

- Works on Windows only (uses System.Speech assembly)
- Plays through the default audio output device
- No external dependencies required
