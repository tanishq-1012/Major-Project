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
