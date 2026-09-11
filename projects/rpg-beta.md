---
layout: project
type: project
image: img/rpg-beta.png
title: "RPG Beta: C++ Adventure Game"
date: 2025-05-01
published: true
labels:
  - C++
  - Object-Oriented Programming
  - JSON
  - Game Development
summary: "A text-based C++ RPG where players create a party of characters and make choices through a story loaded from JSON."
---

# RPG Beta: C++ Adventure Game

## About the Project

RPG Beta is a text-based role-playing game that I worked on for ECE 205 at the University of Hawaii. The game allows players to create a party of characters and move through a story by making different choices.

The story is loaded from a JSON file, which allows the story content to be separate from the main C++ code. The game also uses different character classes and actions depending on the type of character selected.

## Character System

Players can create different types of characters for their party. The available professions include Fighter and Cleric, and characters can have different races such as Dwarf, Elf, Human, or Orc.

Each profession has its own behavior. For example, the Fighter has a sword attack while the Cleric has a healing spell.

This helped me practice using classes and object-oriented programming in C++.

## Story Management

The game uses a JSON file to store the story and its different scenes. The `StoryManager` loads the information from `story.json` and uses it as the player moves through the game.

Players make decisions during different scenes, and their choices determine how the story continues. Some choices can also cause characters to perform actions such as attacking or healing.

Keeping the story in a JSON file also makes it easier to add or change scenes without putting all of the story information directly into the C++ program.

## How I Used C++

The project was separated into different C++ files for different parts of the game.

Some of the main files included:

- `main.cpp` for running the game and managing the player's party.
- `Fighter.cpp` and `Fighter.hpp` for the Fighter character.
- `Cleric.cpp` and `Cleric.hpp` for the Cleric character.
- `GameCharacter.cpp` and `GameCharacter.hpp` for general character functions.
- `StoryManager.cpp` and `StoryManager.hpp` for managing the story.
- `story.json` for storing the story and scenes.

The project also gave me practice with polymorphism because different character classes can perform different actions while still being part of the same character system.

## Challenges

One challenge was understanding how the different classes connect together. Instead of putting the entire game inside one file, the project separates characters, professions, and story management into different files.

Another challenge was working with JSON and understanding how the C++ program could read story information from another file.

Working through these parts helped me better understand how a larger C++ program can be organized into smaller components.

## My Contribution

My contribution to this project was working on the C++ RPG game and connecting the different parts of the program. I worked with the character system, story management, and the JSON-based story to make the game function correctly.

I also tested the program and worked through problems with the different C++ files and classes. This gave me more practice organizing a larger program and understanding how classes, inheritance, polymorphism, and JSON can work together.

## Source Code

The source code for this project is available in my GitHub repository:

[View RPG Beta on GitHub](https://github.com/mgirgis12/ece205-lab14a-RPGbeta-enter-github-mgirgis12)

## What I Learned

This project helped me improve my understanding of C++ and object-oriented programming. I practiced working with classes, inheritance, polymorphism, header files, and multiple source files.

I also learned how JSON can be used with C++ to store information outside of the program. This project helped me see how different programming concepts can work together to build a complete application.
