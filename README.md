2D Game Platform

Unity 2D platformer template built in C#.
A simple side-scroll platform game demonstrating core mechanics such as player movement, jumping, collisions, and level setup.

<img width="685" height="364" alt="Picture333" src="https://github.com/user-attachments/assets/ddffde4f-4327-4e8c-8e2b-ce61b969599e" />


📌 Table of Contents

🧩 About

🚀 Features

🛠️ Built With

📁 Project Structure

🎮 Gameplay Overview

🧠 How It Works

🏗️ How to Run Locally

📌 Controls

🚀 Improvements & Future Work

🧩 About

This project is a 2D platformer game made with Unity (C#). It serves as both a playable prototype and a learning example for Unity 2D mechanics such as physics, animation, input handling, and scene management.

🚀 Features

✔ Player movement (left/right)
✔ Jumping with physics
✔ Ground detection
✔ Platforms and collision
✔ Scene setup ready for expansion

🛠️ Built With
Technology	Purpose
Unity	Game engine
C#	Programming
Unity Physics2D	Collisions & movement


📁 Project Structure
2dGame_Platform/
├── Assets/                # Game assets (scenes, sprites, scripts)
│   ├── Scenes/            # Unity scenes
│   ├── Sprites/           # Art files (player, platforms)
│   ├── Scripts/           # C# gameplay scripts
│   └── Animations/        # Animation files
├── ProjectSettings/       # Unity project configuration
├── .gitignore
├── README.md

🎮 Gameplay Overview

This project demonstrates fundamental 2D platformer gameplay:

Player controls: move and jump using keyboard input

Physics based movement: smooth acceleration and gravity

Ground & wall collision: prevents clipping through platforms

Scene design: basic tutorial level ready for expansion

🧠 How It Works
Player Movement

The PlayerController.cs script handles:

Horizontal movement using Rigidbody2D

Jumping when grounded

Animation state changes based on input and velocity

Typical movement logic:

float move = Input.GetAxis("Horizontal");
rb.velocity = new Vector2(move * speed, rb.velocity.y);

if (isGrounded && Input.GetButtonDown("Jump")) {
    rb.AddForce(new Vector2(0, jumpForce), ForceMode2D.Impulse);
}

Physics & Collisions

BoxCollider2D and CircleCollider2D components detect collisions

LayerMask filters ground layers for proper ground detection

🏗️ How to Run Locally

Install Unity (recommended version specified in ProjectSettings/ProjectVersion.txt)

Clone the repository

git clone https://github.com/sumeyrakarsavran/2dGame_Platform.git


Open the project with Unity Hub

Open the main scene located in Assets/Scenes/

Press Play in the Unity Editor

📌 Controls
Action	Key
Move Left	A / Left Arrow
Move Right	D / Right Arrow
Jump	Space
Quit	Esc (if implemented)


🚀 Improvements & Future Work

Planned enhancements:

Add enemies with simple AI

Collectible items and scoring

Multiple levels & scene transitions

Sound effects and background music

UI menus (Start, Pause, Game Over)
