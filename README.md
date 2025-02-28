This project is a Flappy Bird AI built using Python, Pygame, and NEAT (NeuroEvolution of Augmenting Topologies). The AI trains a neural network to control the bird and optimize its survival by learning when to jump to avoid obstacles.

Project Overview
The game is a clone of the popular mobile game Flappy Bird, where a bird must navigate through a series of pipes by jumping at the right times. Instead of manual player control, this project uses a machine learning approach with NEAT to evolve a neural network that learns the best strategy over multiple generations.

Key Features
Game Mechanics

A bird moves forward, attempting to pass through randomly generated pipes.
The bird can jump to avoid obstacles, and it falls due to gravity when not jumping.
The base moves continuously to simulate ground movement.
The game ends if the bird collides with a pipe or falls off the screen.
AI Training with NEAT

A population of neural networks is initialized to control multiple birds.
Each network receives input values such as the bird’s height and distance from pipes.
Based on these inputs, the AI decides whether to jump or not.
A fitness function rewards birds for staying alive longer and passing pipes.
The best-performing birds pass their traits to the next generation through neuroevolution.
Game Graphics & UI

Uses Pygame to render birds, pipes, background, and base animations.
Displays score and generation number on-screen.
Neural Network Evolution

Uses NEAT-Python to evolve the AI over 50 generations.
A population of birds competes in each generation, with the best-performing ones evolving to improve survival skills.
The best-performing neural network is displayed after training.
How It Works
The game initializes with multiple birds controlled by different neural networks.
The AI observes the bird’s current height and pipe positions.
Based on its neural network’s output, the bird either jumps or stays in place.
Birds that survive longer and pass more pipes receive higher fitness scores.
The NEAT algorithm selects the best-performing birds, mutates their networks, and evolves the next generation.
The cycle repeats until the AI finds an optimal strategy for survival.
Technologies Used
Python – Programming language for implementing the game and AI.
Pygame – Handles game rendering, animations, and event handling.
NEAT-Python – Machine learning library for evolving neural networks.
Expected Outcome
After training, the AI should be able to play Flappy Bird efficiently, avoiding pipes and surviving for longer durations without human intervention.
