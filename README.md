# SIGNAL / SHIFT — Real-Time Shading Lab

A single-file Three.js night-drive experiment comparing vertex-lit Gouraud shading (1996) with per-fragment Phong shading (2006).

## Run it

Open `index.html` on GitHub Pages, or serve the folder locally (ES modules need HTTP):

```sh
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Controls

- Drag the **Time Machine** slider (or use ← / →) to compare the two shading eras.
- Toggle **Thermal GPU** to visualize a vertex-heavy green pass against a fragment-heavy red pass.
- Press **Ⅱ** or Space to pause the drive.

The moving cyan and magenta overhead lights are evaluated in the hood shader. Gouraud mode computes the highlight at mesh vertices and interpolates the result; Phong mode evaluates it for every fragment.
