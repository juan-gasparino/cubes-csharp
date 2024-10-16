# Cube Containment Detection using Geometric Calculations in C#

This project provides a C# implementation to determine whether one cube is fully contained within another cube using geometric calculations and plane analysis.

## Features

- **3D Geometric Calculations**: The algorithm computes the containment by considering the vertices of the cubes and the planes defined by the cube faces.
- **Plane-Point Relationship**: Uses geometric plane equations to evaluate whether the vertices of one cube are inside the boundaries of another cube.
- **General Cube Support**: Works for cubes with different positions and orientations in a 3D space.
  
## How It Works

1. **Cube Representation**: Each cube is represented by its center coordinates, edge length, and orientation in the 3D space.
2. **Plane Equation**: Each face of a cube can be represented as a plane. The algorithm calculates the equation of each of the six planes of the outer cube.
3. **Point Containment Check**: For each vertex of the inner cube, it checks whether the point lies within the boundaries of the planes formed by the outer cube.
4. **Full Containment**: The inner cube is considered to be fully contained if all vertices of the inner cube lie inside the planes of the outer cube.

## Code Structure

- `Cube.cs`: Contains the class definition for the cube and helper methods to generate vertices and planes.
- `Plane.cs`: Defines the class for plane equations and methods for point-plane relation checking.

## Installation

1. Clone the repository:
   ```bash
   git clone git@github.com:juan-gasparino/cubes-csharp.git
