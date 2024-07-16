Synthetic Instruct Data Creation Agent
This project uses GPT-2 to generate, refine, and evaluate instructional data using a Monte Carlo Tree Search (MCTS) approach. The aim is to create high-quality instructional data through several steps, including content transformation, instruction generation, iterative refinement, and cleaning.

Project Structure
Main Code
The main code consists of several key components and functions:

Imports:

Import necessary libraries such as random, numpy, torch, and transformers.
Helper Functions:

to_device(tensor): Moves tensors to the GPU if available.
MCTS and Node Class Implementation:

Node: Represents a node in the MCTS, with methods for expansion and evaluation.
MCTS: Implements the Monte Carlo Tree Search algorithm.
Initialize GPT-2 Models:

Load GPT-2 tokenizer and model.
Initialize a critic model for response evaluation.
Content Transformation:

Transforms raw data seeds into instructional prompts.
Instruction Generation:

Generates instructional text using GPT-2.
Instruction Refinement:

Iteratively refines the generated instructions to enhance clarity and quality.
Text Cleaning:

Cleans the refined instructions by removing unwanted patterns and ensuring proper formatting.
Remove Repeated Phrases:

Ensures uniqueness of instructional sentences by removing repeated phrases.
Generate Instruction Variations:

Creates variations of instructions for better exploration.
MCTS Integration:

Uses MCTS to select the best instructional data through iterative improvement.
Final Formatting:

Formats the final instructions into a structured and readable format.
Print Final Instructions:

Prints the refined and formatted instructions.
