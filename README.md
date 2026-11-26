# Distraction-Free Focus for macOS

A lightweight macOS app that helps you stay focused by reducing visual distractions on your screen.  
Inactive windows are automatically blurred, keeping your active workspace clear and visually dominant.

## Features

- Automatically blurs inactive windows
- Adjustable blur intensity
- Customizable grain amount
- Configurable blur color / tint
- Smooth real-time updates
- Native macOS look and feel

## Why?

When working with many open windows, visual noise can break concentration.  
This app subtly fades inactive content instead of hiding it, helping you focus while keeping context visible.

## Customization

All visual effects can be tuned to your preference:
- Blur strength
- Grain level
- Color tint

## Platform

- macOS only

## Use Cases

- Programming
- Writing
- Design & creative work
- Deep focus sessions

## URL Control (Focus Mode)

You can start Focus Mode directly via URL, including custom data like duration, icon, and text.

### Scheme

`blurrius://focus`

### Supported Query Parameters

- `duration` / `length` / `s`: total duration in seconds
- `hours` / `h`: hours (used when `duration` is not set)
- `minutes` / `m`: minutes (used when `duration` is not set)
- `seconds` / `sec`: seconds (used when `duration` is not set)
- `icon` / `symbol` / `sf`: SF Symbol name (e.g. `moon.fill`)
- `title`: main title shown in overlay
- `text` / `message` / `subtitle`: optional secondary text
- `finishedText` / `doneText` / `completeText`: text shown when timer ends

### Examples

```bash
open "blurrius://focus?duration=1500"

open "blurrius://focus?hours=0&minutes=25&seconds=0&icon=moon.fill&title=Deep%20Work&text=No%20distractions&finishedText=Done"

open "blurrius://focus?length=90&icon=lock.shield.fill&title=Quick%20Focus"
```

### Notes

- If no duration is provided, a default duration is used.
- `duration` (seconds) has priority over `hours`/`minutes`/`seconds`.
- Invalid or unknown icon names fall back to the default icon.



# _No Warranty_
_This project is provided “as is”, without warranty of any kind, express or implied.
The authors make no guarantees regarding the correctness, reliability, or completeness of the software.
To the maximum extent permitted by applicable law, all warranties, including but not limited to implied warranties of merchantability, fitness for a particular purpose, and non-infringement, are disclaimed.
Use this software at your own risk._
