# 🐜 Artificial Evolution of Ant using AI

## Overview

This project simulates the **evolution and survival behavior** of an artificial ant in a grid-based environment using **Artificial Neural Networks (ANN)** and **Genetic Algorithms (GA)**. Inspired by natural selection and survival of the fittest, the project aims to recreate adaptive and intelligent ant behavior in a constrained virtual ecosystem.
Developed as a **Final Year Major Project** by **Tanishq Sharma** and **Aman Raj**, this work integrates evolutionary computation and AI to model how an artificial agent (ant) learns to find food and survive.

## 📌 Objectives

- Simulate a virtual environment where an ant must find food to survive.
- Train the ant's brain (ANN) to optimize food discovery paths.
- Use Genetic Algorithms to evolve the ant's intelligence over generations.
- Record fitness and behavior improvements over time.
  
## 🧠 Technologies & Concepts Used

- 🐍 Python 3.9
- 🧬 Genetic Algorithms (GA)
- 🧠 Artificial Neural Networks (ANN)
- 🎮 Pygame for visualization
- 📊 Fitness tracking and mutation-based learning

## 📁 Project Structure

| File / Folder            | Description                                                  |
|-------------------------|--------------------------------------------------------------|
| `Ant.py`                | Ant class managing movement, vision, and energy logic        |
| `Environment.py`        | Simulates environment, ant-food interaction, and GA loop     |
| `Food.py`               | Handles food generation, tracking, and competition           |
| `Vector.py`             | Vector utility class for position representation             |
| `settings.py`           | Stores grid, tile size, and other simulation constants       |
| `best_weight.pickle`    | Stores the best-performing ANN model for future use          |
| `Major_project.pptx`    | Presentation slides detailing project overview and results   |
| `Tanishq Final Project Report.pdf` | Full academic project report covering theory, code, and analysis |
| `Major Project Synopsis.pdf` | Project proposal and scope outline                      |

## 🧪 Simulation Details

### Environment
- A 20x20 grid world.
- Food randomly placed in the grid.
- Ants die if they move outside the grid or run out of energy.

### Ant
- Can move in 8 directions.
- Has limited vision range and directional mask.
- Decision-making based on a neural network:
  - 20 input neurons
  - 2 hidden layers: [20, 12]
  - 4 output neurons (representing directions)

## 🧬 Genetic Algorithm Details

1. **Initialization**: Random ANN weights as initial population.
2. **Fitness Function**: Based on food collected before death.
3. **Selection**: Top 50% used as parent pool.
4. **Mutation**: 5% mutation rate; crossover not used.
5. **Elitism**: Top 1% carried to the next generation.
6. **Termination**: After 1190 generations or plateau in improvement.

## 📊 Results

- Best Fitness Achieved: `45592083`
- Maximum Food Eaten by a Single Ant: `45596`
- Total Generations Trained: `1190`
- Visual progress shown through fitness and food-eaten graphs.

## 🚧 Limitations

- Only single-ant interaction modeled.
- Environment is relatively simple and grid-bound.
- Learning is slow due to brute-force nature of GA.

## 🚀 Future Work

- Introduce multiple ants for emergent behavior (e.g., teamwork, colony-building).
- Upgrade from Genetic Algorithm to **Reinforcement Learning** for faster and smarter training.
- Add environment dynamics like obstacles, changing food locations, etc.

## 🧾 Authors

- **Tanishq Sharma** 
- **Aman Raj** 

Department of Computer Science & Engineering,  
MDU Rohtak.
