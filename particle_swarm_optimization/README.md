# Particle Swarm Optimization

Swarm intelligence meets benchmark functions. Watch particles find global minima.

## What's Inside

- **PSO Implementation**: Standard & Adaptive variants
- **Benchmark Functions**: Sphere, Rastrigin, Rosenbrock, Ackley
- **Visualizations**: 3D surfaces, convergence curves, particle trajectories
- **Performance Comparison**: Standard vs Adaptive PSO

## Quick Start

Open `PSO_Colab.ipynb` in Google Colab and run all cells. Everything is self-contained.

## The Gist

Particles "fly" through search space, influenced by:

- Their own best position (cognitive)
- Swarm's best position (social)
- Inertia weight (exploration vs exploitation)

Adaptive PSO dynamically adjusts inertia weight (w: 0.9 → 0.4) for better convergence.

## Results Preview

- **Sphere** (unimodal): Easy, converges fast
- **Rastrigin** (multimodal): Hard, many local minima
- **Rosenbrock** (narrow valley): Tricky navigation
- **Ackley** (multimodal): Complex landscape

Try tweaking `n_particles`, `max_iterations`, `w`, `c1`, `c2` in the playground cell.

---

**Author**: Luân B
