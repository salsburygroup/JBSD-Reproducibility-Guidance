# Fictional GROMACS molecular-dynamics Methods example

This example shows how a conventional GROMACS molecular-dynamics Methods section can be written. The settings are illustrative; authors should report the settings used in their study.

## System preparation

The starting protein coordinates are provided in `systems/system-A-start.pdb`. Missing side-chain atoms were added before simulation, and protonation states were assigned for pH 7.0. The protein was modeled with the CHARMM36m force field and solvated with TIP3P water in a dodecahedral box extending at least 1.0 nm from the protein. Sodium and chloride ions were added to neutralize the system and reach a concentration of 0.15 M. GROMACS 2025.2 was used for system preparation and simulation.

## Simulation protocol

The system was energy-minimized by steepest descent until the maximum force was below 1,000 kJ mol⁻¹ nm⁻¹. Position-restrained equilibration consisted of 100 ps in the NVT ensemble followed by 1 ns in the NPT ensemble at 300 K and 1 bar. Production simulations used a 2 fs time step. Bonds to hydrogen atoms were constrained with LINCS. Long-range electrostatics were treated with particle-mesh Ewald, and short-range electrostatic and van der Waals interactions used a 1.2 nm cutoff. Temperature was controlled with the velocity-rescale thermostat, and pressure was controlled with the Parrinello-Rahman barostat.

## Replication and analysis

Three independent 500 ns production replicas were started with independently assigned velocities and different random seeds. The first 50 ns of each replica were excluded as equilibration. The remaining frames were pooled for the primary analyses, giving 1.35 μs of aggregate production sampling. Coordinates were centered on the protein and made whole across periodic boundaries before analysis. GROMACS commands and analysis scripts are archived under `analysis/`; the manuscript-to-files map links each principal figure and table to its trajectories, inputs, scripts, and plotted data.
