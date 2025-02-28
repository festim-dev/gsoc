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
