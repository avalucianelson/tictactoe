# 4x4 Tic-Tac-Toe AI 👾

## Overview 🎮
This Tic-Tac-Toe AI project showcases an artificial intelligence implementation using the minimax algorithm with alpha-beta pruning to challenge human players in Tic-Tac-Toe! The project features a Python-based graphical user interface (GUI) for interactive gameplay.

## Features ✨
- **Interactive GUI**: Play against an AI directly through a user-friendly graphical interface.
- **Intelligent AI**: Utilizes the minimax algorithm with alpha-beta pruning for efficient and challenging gameplay.
- **Real-Time Feedback**: Displays the game state dynamically and updates after each move, showing both player and AI moves.
- **Game Over Detection**: Detects game over conditions (win, lose, or draw) and displays the result accordingly.
- **Graphing Nodes Evaluated**: After you play, you can generate a graph showing the number of nodes the AI evaluated at each move, both with and without alpha beta pruning. This demonstrates the huge difference in efficiency. Make sure to note that the graph generated is log scale!

## Prerequisites 🔧
To run this application, you need:
- Python 3.6 or higher.
- Tkinter for the GUI (comes pre-installed with Python in most cases).
- Matplotlib and Numpy for generating performance graphs.
To ensure all dependencies are installed, you can use the following pip command:

```bash
pip install matplotlib numpy
```

## Installation & Usage 🖱️
Clone the repository to your local machine:
```bash
git clone https://github.com/yourgithubusername/tictactoe-ai.git
cd tictactoe-ai
```

Execute the following command at the root of the project directory to start the game:

```bash
python gui.py
```

Or, if your system requires: 
```bash
python3 gui.py
```

Use the GUI to make moves against the AI. Click on an empty square to make your move, and the AI will respond on its turn. After you're done playing, a pop-up will let you know who won (O being the AI, X being you the human). If you'd like, you can click the button to "Plot Node Counts" and see a graph of the number of nodes evaluated by the AI, both with and without alpha-beta pruning. Please note that you'll have to click the button each time you'd like an updated graph, and restarting the program will mean your graph will not be able to update further.

**Note:**
If you encounter any issues with Tkinter not being recognized, it may be because it's not installed with your Python installation (common in some virtual environments or specific Python installations on Linux). You can typically install it via your package manager (for Linux) or by ensuring you have the official version of Python installed which includes Tkinter.


## How It Works 🤖
- **Minimax Algorithm**: The minimax algorithm is used to simulate decision-making for two-player games. By creating a game tree, it anticipates potential future moves and chooses the optimal path by minimizing the possible loss for a worst-case scenario.

- **Alpha-beta Pruning**: Alpha-beta pruning enhances the minimax algorithm by reducing the number of nodes evaluated, thereby speeding up decision-making by effectively pruning branches that will not influence the final decision.

# Visualizations 👓

## Flowchart 🦦
Here's a flowchart that visualizes the program generally. 

![Flowchart](tictactoe4x4flowchart.svg)

## Quick GIF Demo 👀
I recommend you play my game! But here's a quick peek at what it looks like, in case you're curious. 

![Gameplay Demo](4x4gameplaydemo.gif)

## Example Graph 📉
Here's a look at an example graph visualizing the number of nodes evaluated over 10 games. As you can see, there's a significant difference in the number of nodes exapanded with alpha beta pruning vs without. Be sure to note this is a log scale - so the difference between the blue and red lines is bigger than it seems! 

![Example Graph](example_nodesexpanded_graph.png)


Happy tic-tac-toeing! 
Xoxo ❤️ (get it?)
