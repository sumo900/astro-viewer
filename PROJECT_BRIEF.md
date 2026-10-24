# Solar System VR — Project Brief

## Goal

Create a small educational website for exploring a stylized solar system in A-Frame. The primary target is Meta Quest Browser, with a desktop preview.

## MVP requirements

- Show the Sun and all eight planets in an immersive space scene.
- Use intentionally non-scale sizes and distances so the whole model is easy to see and explore.
- Animate planetary orbits and rotation.
- Provide controls to play/pause motion and switch between artistic speed and real-speed modes.
- Support planet selection by gaze/cursor and VR controller trigger.
- Show a selected body's name and a few student-friendly facts. Show labels when a body is selected.
- In VR, keep the model stationary in the virtual scene so visitors can physically walk around it.
- On desktop, keep the camera still until a planet is selected, then move closer to focus on it. Provide a way to return to the overview.

## Technical direction

- A-Frame with plain HTML, CSS, and JavaScript.
- Frontend-only; no backend for the initial version.
- Keep implementation small and approachable for a student project.
- Planet visuals use lightweight, stylized spheres rather than complex meshes. NASA texture maps can be added once appropriate map assets and their attribution are verified.

## Out of scope for the first version

- Additional moons.
- Detailed scientific simulation.
- Complex navigation.
- Realistic scale or materials.

## Decisions and open questions

- **Real-speed mode:** Use actual orbital periods/rates. Movement will be very slow; the artistic mode is for visibly demonstrating the orbits.
- **VR placement:** Use a fixed model in a virtual VR scene. Visitors can physically walk around it within their play area; this is not room-anchored passthrough AR.
- **Planet assets:** No user-provided 3D files are required. The MVP uses colored sphere materials; NASA texture maps are a possible follow-up after source and attribution review.