# Warfare - Multiplayer Java Server Game

## Overview

**Warfare** is a multiplayer Java server game that leverages a RESTful API architecture. Players join the game by selecting a weapon and are then launched into a random part of the map. The server manages player interactions, map updates, and game logic, while clients communicate through HTTP requests to perform actions in the game.

## Features

- **Multiplayer Gameplay:** Support for multiple players interacting in a dynamic environment.
- **Weapon Selection:** Players choose from a variety of weapons before starting the game.
- **Random Map Placement:** Players are placed in random positions on the game map after weapon selection.
- **RESTful API:** The game operates with a RESTful architecture where players communicate with the server via HTTP requests and receive JSON responses.
- **Server-Client Interaction:** The server processes game logic, while clients send and receive updates via the API.

## Getting Started

### Prerequisites

- **Java 11 or higher**: Ensure Java is installed:
    ```bash
    java -version
    ```
- **Maven**: Required for dependency management and building:
    ```bash
    mvn -v
    ```

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo/warfare-java-server.git
    cd warfare-java-server
    ```

2. Build the project:
    ```bash
    mvn clean install
    ```

3. Run the server:
    ```bash
    java -jar target/warfare-java-server.jar
    ```

### Configuration

Server settings like port, max players, and map size can be modified in `config.properties` (located in `src/main/resources`).

Example:

```properties
server.port=8080
max.players=20
map.size=500
