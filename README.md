# Rubik's Cube Solver Project

This is a C++ implementation of a Rubik's Cube solver that uses various search algorithms and pattern databases to efficiently solve Rubik's Cube configurations.

## Project Structure

The project is organized into several main components:

### Model
Contains different representations of the Rubik's Cube:
- **RubiksCube.h** - Base abstract class defining the interface
- **RubiksCube3dArray.cpp** - 3D array representation
- **RubiksCube1dArray.cpp** - Flattened 1D array representation
- **RubiksCubeBitboard.cpp** - Bitboard representation for speed

### Solver
Contains various search algorithms to solve the cube:
- **DFSSolver.h** - Depth-First Search
- **BFSSolver.h** - Breadth-First Search
- **IDDFSSolver.h** - Iterative Deepening DFS
- **IDAstarSolver.h** - IDA* (advanced heuristic search)

### PatternDatabases
Advanced techniques for faster solving:
- **CornerPatternDatabase.h** - Pattern database for corners
- **PermutationIndexer.h** - Indexes permutations efficiently
- **NibbleArray.h** - Compressed storage for database

## Key Features
- Multiple cube representations for comparative performance
- Various search algorithms with increasing sophistication
- Corner pattern database for efficient heuristic estimation in IDA*
- Ability to randomly shuffle and solve cubes
- Support for all standard Rubik's Cube moves (F, B, U, D, L, R and their variations)

## Implementation Details
The project implements:
- Efficient cube state representation and move application
- Hash functions for cube states to enable memoization
- Optimized pattern database generation and lookup
- Advanced corner indexing and orientation tracking

## Usage
The `main.cpp` file contains examples of how to use the different components to shuffle and solve Rubik's Cubes using the various algorithms.

