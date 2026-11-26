# Apex Ride

An endless 3D motorbike racer in the browser, inspired by motorcycle racing. Ride a sport bike down a curving highway forever, lean through the corners, weave through traffic, and watch the time of day change as you go.

**Play:** https://rohithparjane.github.io/apex-ride/
(or serve this folder locally, e.g. `python3 -m http.server`, and open `http://localhost:8000`; it needs a web server because it uses ES modules)

## Levels: time of day

Every 3.5 km is a new level, cycling **Morning → Day → Evening → Night** and back to morning, forever. The sky, sun or moon, fog, shadows, street lamps, headlights, stars and distant city lights all blend smoothly from one time of day to the next, and traffic gets heavier and faster each level. On night levels there are distant thunderstorms.

## Controls

| Action | Keyboard | Touch |
| --- | --- | --- |
| Throttle | W / ↑ | GAS |
| Brake | S / ↓ | BRAKE |
| Lean left / right | A D / ← → | ◀ ▶ |
| Camera (Chase / Cockpit / TV) | C | CAM button |
| Pause | P / Esc | II button |
| Sound | M | SOUND button |

## Features

- Lean physics: the bike leans into corners (up to about 57°) with a cornering assist, and the lean angle is shown live on the HUD.
- Six-speed auto gearbox, rev counter and a synthesized engine and wind sound.
- **Chase cam**, a **cockpit cam** with working twin round gauges, and a trackside **TV cam**.
- Traffic in three lanes with lane changes and indicators, plus oncoming traffic on the other carriageway.
- **No divider:** cross the painted median and ride the wrong way into oncoming traffic for **4x points**. Dodging an oncoming car closely is a **head-on miss** (+300 x combo).
- Scoring: distance points, overtakes, and **near-miss combos** (up to x8). Crashing resets your ride score; the best score is saved in your browser.
- Real-time shadows, sky reflections on paint and metal, drifting clouds, bloom on lights, a procedural endless road with hills and curves, guardrails, a painted median, street lamps, power pylons, overhead signs and trees.

## Tech

Plain HTML and JavaScript with [Three.js](https://threejs.org) (bundled in `vendor/`, MIT license, see `vendor/THREE_LICENSE`). No build step.
