# Lem-in Project

## Overview

Lem-in is a project that simulates the movement of ants from a start room to an end room through a graph of interconnected rooms. The goal is to find the optimal paths and manage the movement of ants in the most efficient way. This project involves reading input data, creating a graph, finding all possible paths, and simulating the movement of ants.

## Features

- **Input Parsing:** Reads input from a file and extracts the number of ants, room coordinates, and links between rooms.
- **Graph Creation:** Constructs a graph from the parsed input data.
- **Pathfinding:** Finds all possible paths from the start room to the end room.
- **Ant Movement Simulation:** Simulates the movement of ants along the found paths, ensuring no collisions in rooms and paths.

## Usage

1. Compile and run the program with an input file:
    ```sh
    go run . example.txt
    ```
2. Ensure the input file follows the required format:
    ```
    [number_of_ants]
    [room_name] [x_coordinate] [y_coordinate]
    ...
    [room_name] [x_coordinate] [y_coordinate]
    ##start
    [start_room_name] [x_coordinate] [y_coordinate]
    ##end
    [end_room_name] [x_coordinate] [y_coordinate]
    [room1-room2]
    ...
    [roomN-roomM]
    ```

## Example

Example input file `example.txt`:
10
##start
A 1 2
B 2 3
C 3 4
D 4 5
##end
E 5 6
A-B
B-C
C-D
D-E
A-D
