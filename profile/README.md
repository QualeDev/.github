<p align="center">
  <img src="https://quale.dev/assets/logo_light.svg" alt="Quale" width="200" />
</p>

<p align="center">
  <strong>Evolve neural networks to solve real-world problems.</strong>
</p>

<p align="center">
  <a href="https://quale.dev">Website</a> &middot;
  <a href="https://quale.dev/docs/">Documentation</a> &middot;
  <a href="https://quale.dev/research/">Research</a>
</p>

---

Quale is a neuroevolution platform that evolves connectome-based neural networks using NEAT (NeuroEvolution of Augmenting Topologies). Write a `.quale` file describing your domain - sensors, actuators, physics, scoring - and the engine evolves brains that learn to solve it.

No training data. No gradient descent. No labeled datasets. Just selection pressure and millions of generations.

### Repositories

| Repo | Description |
|------|-------------|
| **[Engine](https://github.com/QualeDev/Engine)** | Core evolution engine, bytecode VM, parser, CLI. Go + C (CUDA/OpenCL) |
| **[App](https://github.com/QualeDev/App)** | Desktop GUI for running experiments. Wails + Svelte |
| **[Frontend](https://github.com/QualeDev/Frontend)** | [quale.dev](https://quale.dev) website, research papers, wiki docs. Astro + Starlight |
| **[VSCode](https://github.com/QualeDev/VSCode)** | VS Code extension - syntax highlighting, snippets, comment system |
| **[Run](https://github.com/QualeDev/Run)** | [quale.run](https://quale.run) - browser-based experiment viewer and brain inspector |

### What makes Quale different

- **Domain-specific language** - `.quale` files express entire simulations: world topology, perception, physics, state machines, fitness scoring. Zero Go or C required.
- **Bytecode VM** - One source file compiles to bytecode that runs identically on CPU and GPU. No code duplication.
- **GPU acceleration** - CUDA (NVIDIA) and OpenCL (Intel/AMD) backends evaluate thousands of brains in parallel.
- **Connectome architecture** - Brains have regions, plasticity, and gain modulation inspired by computational neuroscience.

### Demo scenarios

- **Human Factors** - Safety modelling on a route topology with entity interactions, state machines, and dynamics
- **Network Security** - Intrusion detection with per-record fitness and classification scoring
- **Survival** - Grid-world agents with directional sensing, resource consumption, and foraging
