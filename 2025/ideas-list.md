# ⚡️ GSoC 2025 Project Ideas ⚡️

---

Thanks for your interest in applying for Google Summer of Code with FESTIM. We welcome applications from all backgrounds, identities, and abilities and encourage applications from under-represented groups in tech.

## About FESTIM

[FESTIM](https://festim.readthedocs.io/) is an open-source tool for simulating hydrogen transport in materials, with applications in nuclear fusion, hydrogen storage, and beyond. It is built on [FEniCSx](https://fenicsproject.org/) and leverages finite element methods to model diffusion, trapping, and surface interactions.

## Getting Started

This guide illustrates a few steps that’ll help you get acquainted with FESTIM:

- Check out the [FESTIM documentation](https://festim.readthedocs.io/) for an introduction.
- Follow the [installation guide](https://festim.readthedocs.io/en/latest/installation.html) and set up the development environment.
- Explore the example simulations available in the [FESTIM repository](https://github.com/festim-dev/FESTIM).
- Look at the issues labeled [‘good first issue’](https://github.com/festim-dev/FESTIM/issues?q=label%3A%22good+first+issue%22) to get started contributing.

Please find project ideas listed below! 👇🏻

## Project Idea I - Coupling FESTIM with OpenFOAM for Multiphysics Simulations

> **Abstract 🗂**

Hydrogen transport in materials is affected by advection when a fluid is present, such as in fusion reactor cooling systems or hydrogen storage applications. Currently, FESTIM lacks built-in support for advection. OpenFOAM is a widely used computational fluid dynamics (CFD) solver that can model fluid flow. This project aims to couple OpenFOAM with FESTIM to enable the simulation of hydrogen transport in flowing fluids by incorporating advection terms.

This integration will allow FESTIM to:
- Simulate hydrogen transport in complex geometries with advection.
- Improve the accuracy of hydrogen retention and permeation predictions in fusion applications.
- Provide a framework for multiphysics coupling between finite element and CFD solvers.

> **Tasks 📝**

- Investigate available coupling strategies between FEniCSx and OpenFOAM.
- Implement a prototype interface between FESTIM and OpenFOAM for simple geometries.
- Extend FESTIM's governing equations to include advection terms.
- Validate the implementation using benchmark cases with known solutions.
- Document the approach and create example simulations for the FESTIM community.

> **Extended Tasks 📝**

- Optimize the coupling strategy for efficiency and scalability.
- Test the implementation on realistic fusion-relevant cases.
- Integrate coupling with other solvers, such as OpenMC for neutron transport.

> **Project Length ⏰**

175 hours

> **Priority ⏩**

Medium

> **Complexity 👨🏻‍💻**

High

> **Potential Mentors 😇**

- [Remi Delaporte-Mathurin](mailto:remidm@mit.edu)
- [Jorgen Dokken](mailto:dokken@simula.no)

> **Related Links 🔗**

- [FESTIM GitHub Repository](https://github.com/festim-dev/FESTIM)
- [OpenFOAM Official Website](https://www.openfoam.com/)
- [FEniCSx Documentation](https://fenicsproject.org/)

## Project Idea II - Coupling FESTIM with OpenMC for Neutronics Integration

> **Abstract 🗂**

Understanding the effects of neutron irradiation is crucial for predicting material behavior in nuclear fusion reactors. OpenMC is a state-of-the-art Monte Carlo code that performs neutron transport simulations and can calculate heat deposition and tritium production rates. This project aims to couple OpenMC with FESTIM to enable the import of neutron-induced heat sources and tritium production rates into FESTIM simulations. This integration will enhance FESTIM's capability to model the impact of neutron irradiation on hydrogen transport in materials.

> **Tasks 📝**

- **Investigate Coupling Strategies:** Research existing multiphysics coupling methodologies between OpenMC and other simulation tools, such as MOOSE, to inform the development of a coupling interface with FESTIM. ([cardinal.cels.anl.gov](https://cardinal.cels.anl.gov/tutorials/openmc_solid.html?utm_source=chatgpt.com))

- **Develop Coupling Interface:** Implement a robust interface that facilitates the transfer of neutron heating and tritium production data from OpenMC to FESTIM.

- **Extend FESTIM Functionality:** Modify FESTIM to incorporate neutron-induced heat sources and tritium production rates into its simulations.

- **Validation and Testing:** Validate the coupled simulation framework against benchmark problems and experimental data to ensure accuracy.

- **Documentation and Tutorials:** Document the coupling process and develop tutorials to assist users in utilizing the new features.

> **Extended Tasks 📝**

- **Optimization for Performance:** Enhance the efficiency of data transfer and simulation runtime for large-scale problems.

- **Application to Fusion Reactor Models:** Apply the coupled OpenMC-FESTIM framework to realistic fusion reactor component simulations to assess material performance under neutron irradiation.

> **Project Length ⏰**

175 hours

> **Priority ⏩**

High

> **Complexity 👨🏻‍💻**

High

> **Potential Mentors 😇**

- [Remi Delaporte-Mathurin](mailto:remidm@mit.edu)
- [Jon Shimwell](mailto:jon@proximafusion.com)

> **Related Links 🔗**

- [FESTIM GitHub Repository](https://github.com/festim-dev/FESTIM)
- [OpenMC Official Website](https://openmc.org/)
- [OpenMC-MOOSE Coupling Tutorial](https://cardinal.cels.anl.gov/tutorials/openmc_solid.html)
- [OFELIA example code coupling OpenMC with FEniCSx](https://ermete-lab.github.io/MP-OFELIA/intro.html)
