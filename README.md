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

## Focus Mode via URL

The URL scheme is `blurrius://`.

### Start Focus

```text
blurrius://focus
blurrius://focus?duration=300
blurrius://focus?hours=1&minutes=30&title=Deep%20Work&message=No%20distractions&icon=brain.head.profile
```

Supported parameters for `focus`:

- `duration` / `length` / `seconds` / `s`
- or combined: `hours` / `h`, `minutes` / `m`, `seconds` / `sec`
- `title`
- `message` (`text`, `subtitle`)
- `icon` (`symbol`, `sf`)
- `finishedText` (`doneText`, `completeText`)

### Stop Focus

```text
blurrius://focus/off
blurrius://focus/disable
blurrius://off/focus
```

### Conflict Protection

If a Focus session is already active, new `focus` start URLs are intentionally ignored.

This prevents multiple sessions from being registered or overwriting each other.



# _No Warranty_
_This project is provided “as is”, without warranty of any kind, express or implied.
The authors make no guarantees regarding the correctness, reliability, or completeness of the software.
To the maximum extent permitted by applicable law, all warranties, including but not limited to implied warranties of merchantability, fitness for a particular purpose, and non-infringement, are disclaimed.
Use this software at your own risk._
