# Lab3-Part1-ChristianToliver
### Step 1
There was little to no change in the display. The original lookAt() placed the camera at (0, 0, 10) looking toward the origin, while translate(0, 0, -10) moves the scene 10 units away along the Z-axis. In this case, both transformations made a similar view.

### Step 2
When both lookAt() and translate() are removed, the coordinate axes are no longer visible and the canvas appears blank because there is no viewing transformation moving the scene into the camera's visible area.

### Step 4

**Experiment A — 512 x 256:**  
The display became stretched horizontally. The X-axis appeared longer because the perspective projection was still using an aspect ratio of 1.0 even though the canvas was wider than it was tall.

**Experiment B — 256 x 512:**  
The display became stretched vertically. The Y-axis appeared longer because the perspective projection was still using an aspect ratio of 1.0 even though the canvas was taller than it was wide.

**Experiment C:**  
After changing the aspect ratio to `canvas.width / canvas.height`, the scene kept the correct proportions with both canvas sizes.
### Step 10
If I wanted to keep the X-axis and Y-axis in their original orientation while still seeing the tops of the cubes, I would change the camera view using lookAt() instead of rotating the entire scene. This would have the camera look down at the cubes while keeping the coordinate axes in their original orientation.