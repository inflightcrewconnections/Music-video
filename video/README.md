# Jesus, You're My One Thing: lyric video

HyperFrames project for Sean Slayton's lyric video (1920×1080, 30 fps, 4:59.8).

## Change a lyric or its timing

1. Edit `lyrics.json`. Each line has `t`, the time in seconds when it is sung.
2. Run `node build.mjs`, which regenerates `index.html`.
3. Preview with `npm run dev`. Check with `npm run check`.

## Render

```bash
npm run render                                              # high quality → renders/video.mp4
npx hyperframes render . -q draft -o renders/preview.mp4    # faster draft
```

## Files

- `lyrics.json`: lyric lines, timings, and section moods (verse / chorus / bridge …)
- `build.mjs`: generates `index.html` (look, motion, and the heartbeat pulse)
- `audiomap.json`: beat and energy analysis of the song (HyperFrames music-to-video analyzer)
- `assets/`: song, fonts (Cormorant Garamond and Montserrat, SIL OFL), and a local copy of GSAP
