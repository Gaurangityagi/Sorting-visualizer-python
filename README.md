# Sorting-visualizer-python
This is a sorting visualiser using python programming and Pygame for the interface.
Here's a basic `README.md` file for your sorting visualization project:

---

# Sorting Algorithm Visualization

This project is a visualization tool for understanding sorting algorithms using "Pygame". The tool allows you to visualize sorting algorithms such as Bubble Sort and Insertion Sort with a variety of color gradients.

## Table of Contents

- FEATURES
- INSTALLATION
- USAGE
- MAIN FUNCTION 
- CONTROLS

## Features

- **Real-time visualization** of sorting algorithms (Bubble Sort and Insertion Sort)
- **Interactive controls** to start, reset, and toggle between sorting algorithms
- Visual representation of ascending and descending sorts
- Aesthetic gradient color blocks to represent list values

## Installation

1. Clone the repository:

2. Install the required dependencies:
   
   pip install pygame
   

3. Run the project:
   
   python sorting_visualization.py
   

## Usage

Once you run the script, a window will appear displaying the sorting visualization. You can control the sorting process using the keyboard commands described below.

## Main Functions

### main()
This is the entry point of the program. It sets up the Pygame window, initializes key variables, handles user inputs, and manages the game loop where the sorting visualization runs.

### DrawInformation.__init__(self, width, height, lst)
The DrawInformation class is responsible for managing all the drawing aspects, including the window size, padding, and the list being sorted. The constructor initializes the drawing window and stores the list, colors, and fonts.

### draw(draw_info, algo_name, ascending)
This function clears the screen and redraws the necessary elements like the title of the sorting algorithm, control instructions, and the list to be sorted. It calls `draw_list()` to handle the drawing of the list.

### draw_list(draw_info, color_positions={}, clear_bg=False)
This function draws the current state of the list on the screen. It colors the blocks representing the list's elements with gradient colors. It can also highlight specific elements during sorting with custom colors, passed in through `color_positions`.

### generate_starting_list(n, min_val, max_val)
This function generates a random list of integers between `min_val` and `max_val`, with a length of `n`. The generated list will be visualized and sorted.

### bubble_sort(draw_info, ascending=True)
Implements the Bubble Sort algorithm and visualizes each step. It compares adjacent elements and swaps them if they are in the wrong order. The visualization highlights the currently compared elements. The function uses a generator to allow for real-time visualization during the sorting process.

### insertion_sort(draw_info, ascending=True)
Implements the Insertion Sort algorithm and visualizes each step. It inserts each element into its correct position in the already sorted part of the list. The function highlights the moving elements and allows for real-time visualization using a generator.

## Controls

- R: Reset the list to a new random configuration
- SPACE: Start the sorting process
- A: Sort the list in ascending order
- D: Sort the list in descending order
- I: Switch to Insertion Sort
- B: Switch to Bubble Sort
- Close the window: Quit the program

---

This README provides an overview of the project, along with descriptions of the key functions and usage instructions. You can modify it further if needed such as more sorting algorithms can be added!
