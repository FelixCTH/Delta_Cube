# Delta_Cube: Cube Density Interpolation and Subtraction

This Python utility provides a robust framework for interpolating and subtracting electron density data from Gaussian `.cube` files with differing spatial grids. It ensures accurate alignment of molecular coordinates and volumetric data, making it ideal for comparative analysis, such as difference density visualization or reaction-induced charge migration studies.

## 📌 Features

- Reads Gaussian `.cube` files with full metadata retention
- Interpolates a secondary density grid onto a reference grid using `scipy.interpolate.RegularGridInterpolator`
- Subtracts volumetric electron densities
- Outputs a new `.cube` file with proper molecular alignment
- Preserves atomic coordinates, origin, and grid metadata

## 🧪 Use Case

Suppose you have two `.cube` files (`file1.cube`, `file2.cube`) corresponding to different molecular states or quantum chemical calculations. This script will align and subtract them, writing a new cube file `delta_density.cube` that captures their density difference on the same grid.
