# PetriRL: Explainable Reinforcement Learning with Petri Nets  

**PetriRL** is a research framework that integrates **Colored-Timed Petri Nets (CTPNs)** with **Reinforcement Learning (RL)** to solve complex scheduling and optimization problems in **Flexible Manufacturing Systems (FMS)** and beyond.  

Developed as part of my PhD on *Explainable Model-Based Reinforcement Learning for Discrete Event Systems*, PetriRL provides a **formal, modular, and reproducible** approach to dynamic scheduling, intralogistics, and decision-making under uncertainty.  

## Core Idea  

PetriRL bridges **Petri net modeling** and **RL-based decision-making**:  

- **Petri Nets** provide formal semantics, modular scalability, and explainability via token flow and graphical structure.  
- **Reinforcement Learning** provides adaptability, generalization, and efficient online decision-making under dynamic conditions.  
- **Dynamic Action Masking** (from Petri net guard functions) reduces the RL action space, improving sample efficiency and convergence.  

This combination enables **interpretable, scalable, and high-performing RL agents** for scheduling, dispatching, and optimization in discrete event systems.  

---

## PetriRL Environments  

The PetriRL framework is organized into multiple environments, each targeting a different class of problems:  

- 🔹 [**PetriRL Intralogistics**](https://github.com/Sofiene-Uni/Intralogistics)  
  *Dynamic scheduling of AGVs, tool sharing, and shop floor optimization in Flexible Manufacturing Systems.*  

- 🔹 [**PetriRL DJJSP**](#) *(link to repo)*  
  *Dynamic Job Shop Scheduling Problem (DJJSP) with machine breakdowns, variable job arrivals, and stochastic environments.*  

- 🔹 [**PetriRL Hyperheuristics**](#) *(link to repo)*  
  *A super-heuristic framework where RL learns to combine and select dispatching rules for adaptive scheduling.*  

- 🔹 [**PetriRL Multi-Objective Optimization**](#) *(link to repo)*  
  *Combines expert agents and actor-critic RL to solve scheduling problems with multiple objectives (e.g., makespan, tardiness, energy consumption).*  

Each environment is **OpenAI Gym-compatible**, comes with **benchmarks** (Taillard + custom large-scale instances), and is designed for **reproducibility and extension**.  

---

## Why PetriRL?  

✔ **Explainable**: Token flows provide a clear semantic interpretation of RL decisions.  
✔ **Scalable**: Modular Petri net design supports complex and large-scale systems.  
✔ **Efficient**: Action masking reduces search space and improves training efficiency.  
✔ **Adaptive**: RL agents generalize to unseen problems and adapt to disruptions in real time.  
✔ **Research-Ready**: Benchmarks, reproducible pipelines, and Gym compatibility.  

---

## Installation  

Install the core PetriRL package via pip:  

```bash
pip install petrirl
```

Specific environments can be installed or cloned individually from their repositories (see links above).  

---

## Research Context  

PetriRL has been applied to:  
- Flexible Manufacturing Systems intralogistics (AGV + tool sharing).  
- Dynamic job shop scheduling with stochasticity.  
- RL-based hyperheuristics for dispatching rule selection.  
- Multi-objective optimization in scheduling.  

These works are part of my PhD and published in international journals:  

- **Flexible Manufacturing Systems intralogistics: Dynamic optimization of AGVs and tool sharing using Colored-Timed Petri Nets and actor–critic RL with actions masking**  
  [ScienceDirect Link](https://www.sciencedirect.com/science/article/pii/S0278612525001694)  

- **Introducing PetriRL: An innovative framework for JSSP resolution integrating Petri nets and event-based reinforcement learning**  
  [ScienceDirect Link](https://www.sciencedirect.com/science/article/pii/S0278612524000943)  

---

## Citation  

If you use this framework, please cite the associated papers:  

```bibtex
@article{petriRL2025intralogistics,
  title={Flexible Manufacturing Systems intralogistics: Dynamic optimization of AGVs and tool sharing using Colored-Timed Petri Nets and actor–critic RL with actions masking},
  journal={Engineering Applications of Artificial Intelligence},
  year={2025},
  author={Sofiene ...}
}

@article{petriRL2024intro,
  title={Introducing PetriRL: An innovative framework for JSSP resolution integrating Petri nets and event-based reinforcement learning},
  journal={Engineering Applications of Artificial Intelligence},
  year={2024},
  author={Sofiene ...}
}
```

---

## Contributions  

This repository provides the **main entry point** to PetriRL, including:  
- The **core PetriRL package** (`pip install petrirl`).  
- Links to specialized environments.  
- Documentation and research context.  
- Benchmarks and reproducible pipelines for evaluation.  
