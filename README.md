# Slopocalypse Now!

An industrial hip-hop release by **Meat Proxy** (`@Meat_Proxy`). This v1.0 package contains the corrected song audio, the supplied master lyrics, timed lyric/subtitle files, and square cover art.

## Files

| File | Description |
| --- | --- |
| `audio/Slopocalypse_Now.flac` | Lossless 48 kHz, 16-bit stereo encode of the corrected PCM WAV master. |
| `audio/Slopocalypse_Now.mp3` | Corrected MP3 export with its original MPEG audio frames preserved. |
| `lyrics/lyrics.txt` | Supplied intended master lyrics, preserved byte for byte. |
| `lyrics/lyrics.lrc` | 88 performed lines timed to the corrected recording, with clear cues for gaps. |
| `lyrics/subtitles.srt` | 88 full-song subtitle cues timed to the corrected recording. |
| `artwork/cover.png` | 2000 × 2000 square release cover from original project artwork. |
| `LICENSE.md` | CC BY 4.0 terms and attribution guidance. |
| `CREDITS.md` | Release credits and provenance. |
| `SHA256SUMS` | SHA-256 checksums for every other file in this package. |

The corrected PCM master runs **4:13.866**. The FLAC was encoded from that WAV, not from the MP3. The MP3 retains the verified corrected export's MPEG audio frames; its metadata was rewritten for this release. Both audio files report only **Title: Slopocalypse Now!** and **Artist: Meat Proxy** as tags. The cover PNG has no embedded text, author, software, time, or EXIF metadata.

For metadata privacy, the MP3's technical gapless header retains only a generic four-byte codec marker. Redacting its encoder version leaves that header's ancillary checksum mismatched. FFmpeg still decodes the MP3 with the original timing and identical PCM output; a strict third-party player may handle gapless playback differently.

## Lyric timing note

The audio is the timing reference; `lyrics.txt` is the untouched intended-text reference. The LRC and SRT use the current local alignment, which is marked **machine-provisional and needs a full listening review**. At approximately **03:14.620–03:17.030**, the performed bridge line **“Looks good to MEEEE”** appears in the timed files but is absent as a literal line in the supplied master lyrics; the master has a stage direction referring to the sustained “MEEEE.” This difference is retained for review rather than silently changing the master.

## Integrity and size

From this directory, verify the package with:

```sh
sha256sum -c SHA256SUMS
```

Every individual file is smaller than 25 MiB; the largest is the FLAC at about 24.02 MiB. The full music-video MP4 and production source are intentionally outside this compact audio release. Keep `SHA256SUMS` with the files if you copy or upload them.

## Reuse

The audio, lyrics, captions, and cover are available under **[CC BY 4.0](LICENSE.md)**. Credit **Meat Proxy — “Slopocalypse Now!”**, link to the license, and indicate changes when sharing an adaptation.
