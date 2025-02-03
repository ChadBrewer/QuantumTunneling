# Quantum Tunneling Simulation

Welcome to the Quantum Tunneling Simulation project! This repository contains a hybrid quantum-classical simulation built using Q# (for quantum simulation) and C# (as the host program). The simulation models the dynamics of a quantum particle encountering a potential barrier and demonstrates the phenomenon of quantum tunneling.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Visualization](#visualization)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Overview

Quantum tunneling is a nonclassical phenomenon where a particle penetrates a potential barrier even when its energy is lower than the barrier height. This project simulates this effect by numerically solving a simplified version of the time-dependent Schrödinger equation. The Q# component performs the simulation and returns the probability distribution of the particle’s position, while the C# host orchestrates the simulation and displays a visualization using OxyPlot.

## Features

- **Quantum Simulation:**  
  Simulates the time evolution of a quantum state encountering a potential barrier.
  
- **Parameter Control:**  
  Parameters such as evolution time, number of time steps, barrier height, and barrier width can be adjusted.
  
- **Visualization:**  
  Uses OxyPlot within a Windows Forms application to plot the probability density along the spatial grid. (future addition)
  
- **Extensibility:**  
  Modular code structure allows for further enhancements such as decoherence modeling, parameter sweeps, and resonant tunneling simulations.

## Project Structure

```
QuantumTunneling/
├── QSharp/ 
│   └── TunnelingSimulation.qs     # Q# operations for the simulation
├── CSharp/
│   └── Program.cs                 # C# host program integrating with Q#
├── README.md                      # This file
└── QuantumTunneling.sln           # Visual Studio solution file
```

## Requirements

- [.NET SDK](https://dotnet.microsoft.com/download) (version 5.0 or later)
- [Visual Studio Code](https://code.visualstudio.com/) or Visual Studio
- [Microsoft Quantum Development Kit](https://learn.microsoft.com/en-us/quantum/)
- OxyPlot NuGet package (e.g., OxyPlot.WindowsForms) for visualization (future addition)

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/ChadBrewer/quantumtunneling.git
   cd quantumtunneling
   ```

2. **Restore NuGet Packages:**

   In the solution directory, run:
   
   ```bash
   dotnet restore
   ```

3. **Open the Project:**

   Open the folder in Visual Studio Code or your preferred IDE.

## Usage

1. **Build the Project:**

   Use your IDE or run the following command in the solution directory:
   
   ```bash
   dotnet build
   ```

2. **Run the Simulation:**

   Launch the C# host program by executing:
   
   ```bash
   dotnet run --project CSharp
   ```
   
   This will start the simulation and open a Windows Forms window with the visualization of the probability density.

3. **Adjust Parameters:**

   Modify the simulation parameters (evolution time, time steps, barrier height, and barrier width) in the C# code or pass them as arguments (if you implement such functionality) to observe different tunneling behavior.

## Contributing

Contributions are welcome! If you have ideas for additional features (e.g., decoherence modeling, parameter sweeps, double-barrier resonant tunneling), feel free to fork the repository and submit pull requests. Please follow the standard GitHub workflow and ensure your code is well-documented.

## License

NONE, DO AS YOU PLEASE!

## Acknowledgements

- [Microsoft Quantum Development Kit](https://learn.microsoft.com/en-us/quantum/)
- [OxyPlot](https://oxyplot.github.io/)
- Inspirations from quantum mechanics and tunneling research

```

---

Feel free to modify or extend this README document as needed for your project. Simply save the content as `README.md` in your repository’s root folder, commit the changes, and push to GitHub.
