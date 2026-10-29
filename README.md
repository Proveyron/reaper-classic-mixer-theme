# Default 7.0 Classic Mixer — REAPER theme

A REAPER 7 theme that keeps the stock **Default 7.0** look and adds compact,
Classic-1.x-style mixer strips, so dozens of tracks fit on one screen in
two or more rows.

## Download

**[⬇ Download Default_7.0_ClassicMixer.ReaperThemeZip](https://github.com/Proveyron/reaper-classic-mixer-theme/releases/latest/download/Default_7.0_ClassicMixer.ReaperThemeZip)**

Or grab it from the [Releases page](https://github.com/Proveyron/reaper-classic-mixer-theme/releases/latest).

## Install

1. Download `Default_7.0_ClassicMixer.ReaperThemeZip`.
2. In REAPER: **Options → Themes → Load theme…** and pick the file
   (or drag it onto the REAPER window).
3. Open the mixer (`Ctrl+M`). With **Show multiple rows of tracks when size
   permits** enabled in the mixer menu, tracks wrap into rows.

## Mixer layouts

Everything outside the mixer (track panel, transport, envelopes, master) is the
stock Default 7.0 theme. The mixer gets three layouts (each also in 150% and
200%): right-click a mixer strip → **Layout**.

| Layout | Strip | Contents (top → bottom) |
|---|---|---|
| **Classic compact** (default) | 54 px | channel number, track name, 51 px meter with peak readout and dB scale, solo + mute, rec arm |
| **Classic compact fader** | 64 px | same, with a 24 px volume fader to the left of a narrower meter |
| **Classic ultra compact** | 29 px | channel number, track name, 26 px meter, mute, rec arm (no solo) |

Details:

- Dark strips (`#262626`) separated by a small gap (`#333333`); selected tracks
  get the 7.0 white highlight; track colours tint the strip.
- Rec-armed meters are **green** instead of orange: green background, green level
  bar and green scale numbers. Clips still turn the meter and the peak readout red.
- The 7.0 fader background is transparent, so only the fader slot and handle show.

## Built from

- Cockos **Default 7.0** theme as shipped with REAPER 7.83 (`Default_7.0.ReaperThemeZip`).
- Changes are in [`source/rtconfig.txt`](source/rtconfig.txt): macro `drawMcpClassic`
  plus its `Layout` blocks, and the default (unnamed) mixer layout points to it.
- Edited images: `mcp_volbg.png` (all scales), `meter_strip_v.png`, `meter_clip_v.png`.

## License

The Default 7.0 theme is © Cockos Inc and licensed under the
[GNU LGPL v2 or later](https://www.gnu.org/licenses/lgpl.html). This modified
version is distributed under the same license — see [LICENSE](LICENSE).
