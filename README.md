# Mini Museum AR - The Red Fox

A small WebAR "museum exhibit" built with A-Frame and AR.js. Point your phone camera at the Hiro marker and a red fox appears on a display plinth, with a name placard, a bouncing orb you can tap, and a button that shows a fun fact.

**Group number:** [add group number]

**Members:**
- [Member 1]
- [Member 2]
- [Member 3]
- [Member 4]

**Live app (HTTPS):** https://[github-username].github.io/[repository-name]/

## How to use it

1. Open the live link on your phone and allow camera access.
2. Show the Hiro marker (printed, or on a second screen) so the whole black border is visible.
3. The banner at the top turns green when the marker is found and red when it is lost.
4. Tap the bouncing orb to change its colour.
5. Tap the yellow cone to show or hide the fact card.

## Features

| Requirement | Where it is in the app |
| --- | --- |
| Hiro marker scene (4+ objects, 2+ primitives, one `<a-text>`) | Floor plane, cylinder plinth, box placard, sphere orb, cone button, plus `<a-text>` labels |
| Animation (2+ objects, different properties) | Fox rotates (rotation), orb bounces (position), cone pulses (scale) |
| 3D model (not the duck) | Fox glTF/GLB model, credited below |
| Interaction | Orb changes colour (`color-changer`), cone toggles the fact card (`info-toggle`, our own component) |
| Status banner | `marker-status` component changes the banner text and colour on `markerFound` / `markerLost` |
| Hosting | Published on GitHub Pages (HTTPS) and tested on a phone |

## Running it locally

1. Open the project folder in Visual Studio Code.
2. Right-click `index.html` and choose **Open with Live Server**.
3. Allow the camera in Chrome and show the Hiro marker.

Camera access only works on `localhost` or HTTPS, so use the live link to test on a phone.

## Credits and licences

**3D model: Fox**
- Low poly fox model by PixelMannen (2014), licensed CC0 1.0 Universal. Source: https://opengameart.org/content/fox-and-shiba
- Rigging and animation by tomkranis (2014), licensed CC BY 4.0. Source: https://sketchfab.com/3d-models/low-poly-fox-by-pixelmannen-animated-371dea88d7e04a76af5763f2a36866bc
- glTF conversion by @AsoboStudio and @scurest (2017), licensed CC BY 4.0.
- Obtained from the Khronos glTF Sample Assets repository: https://github.com/KhronosGroup/glTF-Sample-Assets/tree/main/Models/Fox
- CC0 1.0: https://creativecommons.org/publicdomain/zero/1.0/
- CC BY 4.0: https://creativecommons.org/licenses/by/4.0/

The model is loaded directly from the Khronos repository and has not been modified. Our app only displays it in its default pose and rotates it.

**Libraries**
- A-Frame 1.3.0 - https://aframe.io
- AR.js 3.4.5 - https://github.com/AR-js-org/AR.js
