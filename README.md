# 2D Key Quest: The WizzardsGame

## Project Overview

Welcome to **2D Key Quest: The Wizzardsgame**, a simple 2D adventure game developed primarily in Java. In this game, you control a character tasked with navigating a series of rooms to find hidden keys. These keys are crucial for unlocking doors, with the ultimate goal of reaching the final room and achieving victory!

This project served as an exploration into 2D game development fundamentals, including character movement, collision detection, object interaction, and basic NPC behavior within a tile-based environment. While the game is a foundational prototype, it lays the groundwork for more complex adventures.

## Gameplay Features

* **Key Collection:** Your main objective is to collect keys by colliding with specific Non-Player Characters (NPCs). While the first key might be easily obtained, ***subsequent keys from the same NPC may require more persistent interaction or repeated engagement***.

* **Door Unlocking:** Collected keys allow you to open locked doors, granting access to new areas and progressing through the game.

* **Dynamic NPCs:** The world is populated by various NPCs (currently two types, with potential for more) that move around the map, adding life and challenge to the environment.

* **Room-Based Progression:** The game features multiple rooms, each potentially holding new challenges and keys, leading to the final objective.

* **Winning Condition:** Successfully unlocking the last door leads to victory!

* **Power-Up Items:** Discover and collect special items within the game world that provide temporary boosts, such as increased character speed.

* **On-screen UI:** A user interface displays crucial game information, including:

    * **Current Time:** Tracks the elapsed time during your adventure.

    * **Key Count:** Shows the number of keys you currently possess.

    * **Final Time:** Upon winning, your total completion time is displayed.

## Technical Details

The game's core logic and rendering are entirely handled in **Java**, leveraging standard Java Swing/AWT for graphics.

### Map Generation

An original design choice for map creation involved **Python scripts**. These scripts were used to:

* **Tile the Map:** Generate the tile-based structure of the game world.

* **Create the Matrix:** Produce the underlying matrix representation of the map, which is then utilized by the Java game for rendering and collision detection.

*(Note: The map generation process is a separate utility; the game itself consumes the generated map data.)*

### Design Considerations

This project was developed with a focus on learning and implementing core game mechanics. As such, some aspects, particularly the map design and collision system, are relatively straightforward and could be expanded upon in future iterations. The current map is not extensively complex due to initial tiling limitations.

## How to Play

1.  **Movement:** Use the arrow keys (or WASD, if implemented) to move your character around the 2D map.

2.  **Interact:** Collide with specific NPCs to obtain keys or pick up power-up items.

3.  **Unlock Doors:** Walk into locked doors with the required keys in your inventory to open them.

4.  **Win:** Unlock the final door to complete the game!

## Getting Started

To compile and run the game, you will need a Java Development Kit (JDK) installed on your system.

1.  **Prerequisites:**

    * Java Development Kit (JDK) 8 or higher.

2.  **Clone the Repository:**

    ```
    git clone <repository_url>
    cd <your-game-directory>


    ```

3.  **Compile the Java Code:**
    Navigate to the `src` directory (or wherever your Java source files are located) and compile:

    ```
    # Example, adjust path if your source files are in a different sub-directory
    javac main/*.java entity/*.java object/*.java tile/*.java # Add all relevant packages


    ```

    *(You might need to compile each package separately or use an IDE like IntelliJ IDEA or Eclipse which handles compilation automatically.)*

4.  **Run the Game:**
    After successful compilation, run the `Main` class:

    ```
    java main.Main


    ```

## Future Enhancements

* **Expanded Map Design:** Implement more complex and varied tile sets and map layouts.

* **Improved Collision System:** Refine collision detection for more nuanced interactions.

* **More NPC Types:** Introduce additional NPC behaviors, challenges, and interactions.

* **Inventory System:** Develop a more robust inventory for managing keys and other potential items.

* **Sound Effects and Music:** Add audio to enhance the gameplay experience.


## Acknowledgements / Inspiration

This project was developed with significant inspiration from RyiSnow's 2D Java Game Development Tutorial Series (https://www.youtube.com/watch?v=om59cwR7psI&list=PL_QPQmz5C6WUF-pOQDsbsKbaBZqXj4qSq). Their clear explanations and guidance were instrumental in understanding the core game loop, tile rendering, and basic entity management.

## Author

Federico Donati
