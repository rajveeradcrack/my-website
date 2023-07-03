---
sidebar_position: 1
---

# Anarchy Architecture

## Introduction & Goals

### Game introduction

It's a battle royale that spans across various times and dimensions, with different clans from across the universe competing to become the ultimate masters of the universe. In its first season, Earth serves as the ground zero for this battle. To learn more about the game, please refer to the Game Design Document. 

### Game goals

Our goals is to create a battle royal game in a futuristic settings where players can explore different characters and rich back stories. It is inspired by PUBG. Further, we plan to make it more entertaining by adding the concept of seasons to it. i.e., S1, S2, etc. For we can keep things refresh for players by introducing new concepts with every season release.

## **Introduction to anarchy game architecture**

![Screenshot 2023-07-03 at 12.49.22 PM.png](..\static\img\Screenshot_2023-07-03_at_12.49.22_PM.png)

### The context level design

This sections explains the Anarchy game architecture. This will covers a high level view of how the game is made, its modules, processes and overall software architecture we choose to keep the game running smoothly. 

In total there are 5 components that take the game from being a concept to actually being deployed to different phones.

- Game design concept
- Unity3D
- Game deployment
- APIs
- 3rd party plugin & libraries

## The architecture explanation

In this section, we will explain each container in depth with each of its moving parts like modules and how they connect with each other.

### Game design concept

The game design concept covers creating the game art like maps, characters modeling them, animations, and other things. These assets are what will gives life to the games and bring them together inside unity3D. All the information about what the maps and characters will look like is given in the game design document and here designers will try to bring that concepts to life by using tools like maya and photoshop and other 3r party assets which we buy from various sources to make the game.  

### Level design

Level design in game development is the process of creating the actual settings and maps where the player interacts with its surroundings. It involves designing the layout of the game levels, including the placement of objects, enemies, and obstacles. The goal of level design is to create an engaging and challenging experience for the player that is both fun and rewarding to play.

### Modeling

Modeling is the process of creating 3D models of characters, objects, and environments that will be used in the game. These models are created using specialized software and can be textured, animated, and manipulated to create a realistic and immersive game world. Modeling is an important aspect of game development as it helps bring the game's design concepts to life and gives players a visual representation of the game's world.

### Animations

Animations is the process of creating movement for characters, objects, and environments within the game. Animations can range from simple movements like walking and running to more complex actions like combat and spell casting. Animations are typically created using specialized software and can be integrated into the game using Unity3D. Animations play a crucial role in making the game more immersive and engaging for players.

### VFX

VFX is the process of creating and integrating special effects into a game to enhance the player's visual experience. This can include effects such as explosions, particle effects, and lighting effects. VFX are typically created using specialized software and can be integrated into the game using Unity3D. They play a crucial role in making the game more immersive and engaging for players.

## Unity3D

Unity3D is a game engine used in game development that provides tools for creating 3D and 2D games. It's an important part of game development as it provides features like 3D model integration, animations, camera, user interface, etc. Unity3D is used throughout the game development process from designing and creating assets to deploying the game on different platforms.

We will integrate the assets we have developed into Unity to bring them to life by animating them and setting them up with other components, such as maps, characters, textures, and more. This involves adding physics to the game and making it interact with other elements. It also requires custom code to be written in Unity.

### Level design

In Unity3D, level design involves creating the physical layout of the level using the editor and then populating it with objects, enemies, and other interactive elements. The level can then be tested within the engine to ensure that it is functioning as intended and that the player experience is enjoyable.

### 3d model integration

3D model integration in Unity3D refers to the process of importing 3D models created using specialized software into Unity3D and integrating them into the game. This involves texturing the models and setting them up with other components like maps, characters, and animations. The process also includes adding physics to the game and making it interactive with other elements. Custom coding may be required in Unity3D for certain features.

### Animations

In Unity3D, animations refer to the process of creating movement for characters, objects, and environments within the game. Animations can range from simple movements like walking and running to more complex actions like combat and spell casting. Animations are typically created using specialized software and can be integrated into the game using Unity3D. Animations play a crucial role in making the game more immersive and engaging for players.

### Camera

In Unity3D, the camera refers to the component that defines the viewpoint through which the player sees the game world. It determines the perspective and field of view of the player's view and can be adjusted to create different visual effects, such as zooming in or out, or changing the angle of the view. The camera can also be used to create cutscenes and other cinematic effects within the game.

### User interface

User interface allows the player to interact with the game, such as menus, buttons, and HUD elements. These elements are typically created using Unity's UI system and can be customized to match the game's design. The user interface is an important aspect of game development as it helps the player navigate the game and provides feedback on their actions.

### Input system

Input systems are the components that handles user input, such as onscreen taps and buttons, and maps them to in-game actions. This allows the player to interact with the game and control their character. The input system can be customized to support different input devices and can be configured to respond to both keyboard and gamepad input.

### VFX

VFX is the process of creating and integrating special effects into a game to enhance the player's visual experience. This can include effects such as explosions, particle effects, and lighting effects. VFX are typically created using specialized software and can be integrated into the game using Unity3D. They play a crucial role in making the game more immersive and engaging for players.

### AI(NPCs)

AI (NPCs) is the implementation of artificial intelligence for non-player characters within the game. This involves programming the behavior and decision-making processes of NPCs so that they can interact with the player and the game environment in a realistic and engaging way. This can include things like pathfinding, decision-making based on the player's actions, and responding to environmental factors like weather or time of day.

### Code integration on Modules

Code integration involves integrating different modules and components into the game engine using appropriate APIs and plugins. This includes integrating lighting and networking components, as well as third-party plugins and libraries like Photon, VFX, and SFX. The game's source code can be designed using SOLID principles and design patterns like Singleton, Strategy, and Observer. Unity3D also offers cross-cutting features like the Unity Performance Reporting (UPR) feature to help optimize game performance. Finally, hardware and infrastructure deployment involves hosting and deploying the game on different platforms.

### API

API in Unity3D refers to the Application Programming Interface which allows developers to interact with the game engine and create custom features and functionality. This can include things like integrating third-party plugins, building custom shaders, or creating AI behaviors. By using the Unity3D API, developers can create a more robust and customized game experience that meets the needs of their specific project.

### Plugins

Plugins in Unity3D refer to third-party libraries or tools that can be integrated with the game engine to provide additional functionality, such as special effects, shaders, and AI behavior. These plugins can be developed by third-party developers or by the Unity community and can be downloaded from the Unity Asset Store. By using plugins, developers can enhance the game's functionality and improve the player experience without having to write custom code from scratch.

### Lighting

In Unity3D, lighting refers to the process of creating and manipulating the lighting within the game environment to create the desired visual effects. This can include setting up lighting sources, adjusting the intensity and color of the light, and adding shadows and other effects. Lighting is an important aspect of game development as it helps to create a more immersive and realistic game world that enhances the player experience.

### Networking

Networking in Unity3D refers to the process of creating and implementing the multiplayer functionality of the game, allowing players to connect and interact with each other online. This involves designing and developing the server-side infrastructure and communication protocols, as well as implementing the client-side networking code in Unity. The networking system in Unity3D enables developers to create complex and scalable multiplayer games that can be played by thousands of players simultaneously.

## The game deployment

Game deployment in Unity3D is the process of deploying the game to different platforms, such as Android, iOS, and desktop. This involves building server components of the game, creating client builds, and integrating APIs like game and analytics/data API. Additionally, it involves testing the game on different platforms to ensure that it runs smoothly and meets the requirements of the platform. Once the game is deployed, it can be made available to the public for download or distribution.

### Server build

Server build is the process of building the server components of the game and creating client builds for different platforms, such as Android, iOS, and desktop.

- Clients
    - Android
    - iOS
- APIs
    - Game API
    - Analytics/Data API

## 3rd party plugin and libraries

- Photon, VFX, SFX, etc.

# **The game development workflow**

At Anarchy, we have developed a game development workflow that allows us to create games from start to finish. Our process includes creating a game design document, using agile development methodologies, and designing a workflow that allows for efficient and effective development. We cover all aspects of game development, such as creating assets and designing levels, programming features, and integrating APIs and plugins. Our workflow is designed to ensure that the game is developed according to a set of quality standards and meets the needs and expectations of our target audience.

Game design document (GDD)

The agile development

### The workflow design

The workflow cover how our team at Anarchy works. We have different teams that covers things from designing to APIs. The below images shows the how we collaborate and the process we follow. 

![game dev workflow copy (1).jpg](..\static\img\game_dev_workflow_copy_(1).jpg)

### The level team

The level team is responsible for creating the game's environment and settings in which the player will interact. They come up with the game design concept, create the art, UI, and other elements needed to bring the environment to life. They design the layout of the game levels, including the placement of objects, enemies, and obstacles. The level team's goal is to create an engaging and challenging experience for the player that is both fun and rewarding to play.

### The modeling team

The modeling team is responsible for creating 3D models of the game's characters, objects, and environments using specialized software. They take the game design concept from the level team and bring it to life by creating complex models for it. These models can be textured, animated, and manipulated to create a realistic and immersive game world. They work with tools like Maya and Photoshop and other 3rd party assets which they buy from various sources to make the game. The modeling team plays an important role in game development as it helps bring the game's design concepts to life and gives players a visual representation of the game's world.

### The UX team

The UX team in game development is responsible for creating the user experience of the game. This includes designing the game's user interface (UI) and user experience (UX), such as menus, buttons, and HUD elements. They are responsible for ensuring that the game's user interface is intuitive and easy to use, and that it provides feedback on the player's actions. The UX team also works on the game's wireframes and flowcharts, which help to define the user experience and ensure that it meets the needs of the target audience. Additionally, they may conduct user testing to ensure that the game's user experience is enjoyable and engaging.

### The animations

The animations team is responsible for creating movement for characters, objects, and environments within the game. They use specialized software to create animations that range from simple movements like walking and running to more complex actions like combat and spell casting. The animations team works closely with other teams like the modeling team to ensure that the animations are integrated seamlessly into the game. They also work with the Unity team to make sure that the animations are properly integrated into the game engine and that they interact with other elements like maps, characters, and VFX. The animations team plays a crucial role in making the game more immersive and engaging for players.

### The unity team

The Unity team is responsible for integrating all of the game's assets and modules into Unity3D, which provides tools for creating 3D and 2D games. They bring the assets to life by animating them and setting them up with other components such as maps, characters, textures, and more. This involves adding physics to the game and making it interact with other elements. The team also writes custom code in Unity3D. Their tasks include level design, 3D model integration, animations, camera, user interface, input system, VFX, AI (NPCs), code integration on modules, APIs, and plugins. They are responsible for ensuring that the game runs smoothly on different platforms and that it meets the quality standards set by the development team.

### The API team

The API team is responsible for creating and managing the game's Application Programming Interface (API). They design, develop and test the APIs and ensure that they are integrated properly into the game engine. They work closely with other teams to ensure that the APIs meet the needs of the development team. Additionally, they may provide documentation and support for other developers who use the APIs in their projects.

### **Game play**

![Wireframe_UI_Flow.jpg](..\static\img\Wireframe_UI_Flow.jpg)

### **The game source code diagram**

In game development, the source code diagram is a representation of the game's code structure. 

### SOLID principles

SOLID principles in game development are a set of guidelines for writing code that is flexible, maintainable, and scalable. The five principles are Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion. By following these principles, developers can write code that is easier to modify and extend, and that is more resilient to changes in the game's requirements.

### Design patterns

**Singleton Design Pattern**

Singleton Design Pattern ensures only one instance of a class is created and can be accessed globally in game development. It's useful for managing resources like audio, graphics, or player data, preventing conflicts and inefficiencies.

**Strategy Design Pattern**

Strategy Design Pattern in game development defines a set of algorithms that can be used to perform a specific task and allows the developer to choose which algorithm to use at runtime. This makes it easy to change the behavior of a game object without changing its class or the code that uses it.

**Observer Design Pattern**

The Observer Design Pattern is used in game development to notify objects of changes to the state of other objects. It defines a one-to-many relationship between objects, where one object maintains a list of its dependents and notifies them automatically of any state changes. In games, this pattern is useful for updating the UI or other game elements based on changes in the game state.

**Hardware and infra deployment**

- Hosting & game deployment

**Cross-cutting features**

UPR unity feature

UPR (Unity Performance Reporting) is a feature in Unity3D that allows developers to collect and analyze data on game performance across different platforms. It provides insights into how the game is performing in terms of frame rates, memory usage, and other key metrics, and helps developers identify and fix performance issues. UPR can be used to optimize game performance and improve the overall player experience.

**Quality tree**

- Quality scenarios