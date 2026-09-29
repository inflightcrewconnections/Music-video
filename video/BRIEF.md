---
workflow: music-to-video
flow: automation
storyboard: no
message: "Jesus is my one thing, my heartbeat"
destination: youtube
aspect: 1920x1080
language: en
length: full song (4:59.8)
angle: lyric video
---

## Intent

A full-length lyric video for the Suno track "Jesus, You're My One Thing" by
Sean Slayton, with a contemporary Christian (CCM) look: reverent, warm, and uplifting.

## Assets

- assets/bgm.mp3: the Suno master, which is the video's audio track.
- lyrics.json: the lyric sheet with per-line timings; build.mjs reads it.

## Customizations

- Light story: night sky (verses) → golden sunrise (choruses) → candlelit cross
  (bridge "Here I am, Lord") → rising light ("Jesus, Jesus, Mighty Savior").
- "Heartbeat" lines draw a gold ECG trace, and the glow behind the lyrics pulses
  lub-dub on the ~68 BPM beat during choruses.

## Notes

- Line timings were derived from the audio (pocketsphinx forced alignment on the
  mix + chroma cross-correlation of repeated sections) because Whisper model
  downloads were blocked in the build environment. The verse and chorus timings are
  cross-checked; the bridge is the least certain. Adjust any line in lyrics.json.
