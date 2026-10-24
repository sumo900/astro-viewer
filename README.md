# Orbit — Solar System Explorer

A small A-Frame solar system you can explore in a desktop browser or Meta Quest Browser. The scene shows the Sun and eight planets with deliberately non-scale distances and sizes.

## Run locally

The page needs to be served over HTTP; opening `index.html` directly as a file will not work reliably with A-Frame/WebXR.

1. From this folder, start a local static server: `python3 -m http.server 8000`.
2. Open `http://localhost:8000` in a desktop browser.

No build step or package installation is required. A-Frame and the display fonts are loaded from CDNs, so the first run needs an internet connection.

## Explore

- Select a planet with the mouse or gaze/cursor; use the controller trigger in VR.
- On desktop, drag to look around. Selecting a planet moves the camera in for a closer view; choose **Back to overview** to return.
- Use the lower controls to pause/play or switch simulation speeds.
- Enter VR using the A-Frame VR button. The model scales down to a room-scale virtual scene; move carefully and stay inside your headset's guardian boundary.

## Simulation notes

- **Artistic speed:** one Earth orbit takes about 60 seconds. The other orbital periods keep their relative proportions. Rotation is independently accelerated for visibility (one Earth spin takes about 10 seconds), so rotation is not time-synchronous with orbit speed.
- **Real speed:** one simulated second equals one real second for orbital motion and rotation. Planet positions use illustrative spacing and do not represent their actual positions in the sky.
- Planet appearances are lightweight, stylized materials rather than photographic surface maps. The model is educational and not to scale.

## Meta Quest Browser

WebXR requires a secure context. For Quest, serve/deploy the site over HTTPS (for example, a static HTTPS host) and open that URL in Meta Quest Browser. A plain `http://` LAN address may not allow VR entry. Headset/browser support and available room-scale movement can vary.