# Ray Casting Visualization

A minimal, interactive demonstration of 2D ray intersection logic built with vanilla JavaScript and HTML5

[Live Demo](https://starryguli.github.io/ray-casting-simulator/)

## Overview

This project simulates a point source emitting rays within a closed square boundary. It calculates the intersection coordinates of each ray against the walls and renders the distance in real-time.

**Key Features:**

- **Interactive Source:** Drag and drop point `B` to move the origin.
    
- **Rotation:** Adjust the projection angle via the UI slider.
    
- **Collision Detection:** Mathematical calculation of vector intersections with bounding box limits.
    
- **Zero Dependencies:** Written in pure JS, no build step required.

## Usage

Simply open `index.html` in any modern web browser.

```
git clone https://github.com/StarryGuli/ray-casting-simulator
```

## Implementation Details

The core logic determines the ray length by comparing distances to vertical and horizontal boundaries:

1. Normalizes the input angle.
    
2. Calculates the distance to the nearest vertical wall (`x=0` or `x=width`).
    
3. Calculates the distance to the nearest horizontal wall (`y=0` or `y=height`).
    
4. Renders the ray using the minimum of the two distances.

## License

MIT