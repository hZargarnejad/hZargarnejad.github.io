# 2D Flow Simulation Around Multiple Circular Obstacles using WaterLily.jl

This project simulates 2D incompressible fluid flow around multiple fixed circular obstacles using [WaterLily.jl](https://github.com/nerdchicken/WaterLily.jl), a GPU-accelerated fluid solver written in Julia. The simulation visualizes the resulting vortex dynamics using a vorticity-based color map, and saves the output as an animated `.gif` file.

## Features

- Multiple fixed circular solid bodies in a uniform inlet flow
- GPU-accelerated simulation using `CuArray` and CUDA.jl
- Visualization of vorticity field
- Export of simulation results as an animated GIF

## Requirements

- Julia 1.6 or later (Julia 1.9+ recommended)
- CUDA-capable GPU with NVIDIA drivers installed
- The following Julia packages:
  - `WaterLily`
  - `StaticArrays`
  - `Plots`
  - `CUDA`

You can install the dependencies via Julia's package manager:

```julia
using Pkg
Pkg.add(["WaterLily", "StaticArrays", "Plots", "CUDA"])
