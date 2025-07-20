# Quantum-Noise-Analysis
A practical investigation into the effects of real hardware noise on quantum computations by comparing ideal simulator results with those from an actual IBM Quantum device.


# Analysis of Noise in Real Quantum Hardware

This repository explores the critical difference between ideal quantum simulations and computations on real, noisy quantum hardware.

The experiment creates a 3-qubit Greenberger-Horne-Zeilinger (GHZ) state, which is a maximally entangled state. In an ideal world, measuring this state should only ever result in `000` or `111`. By running this experiment on both a perfect simulator and a real IBM Quantum device, we can quantify the impact of decoherence and gate errors.

### Comparison of Results

| Ideal Simulator Result | Real Hardware Result (from `ibmq_manila`) |
| :---: | :---: |
| ![Ideal Results](ideal_ghz_plot.png) | ![Noisy Results](noisy_ghz_plot.png) |

**Observations:**
As seen above, the ideal simulation produces only the expected `000` and `111` states. The results from the real hardware show a significant number of erroneous outcomes (e.g., `001`, `101`), demonstrating the challenge that quantum noise presents to building fault-tolerant quantum computers.

**Status:** not started
