# Chapter 2: Basics of Theatre.js

Welcome to the second chapter of our comprehensive guide to Theatre.js! In this chapter, we will cover the core concepts of Theatre.js and write our first script.

## Understanding the Core Concepts

Before we start coding, let's understand some of the core concepts of Theatre.js:

- **Scene**: A scene in Theatre.js is a container for all the elements that make up a part of your story. It can include characters, dialogues, animations, and more.
- **Character**: A character in Theatre.js is an entity that can perform actions and interact with other characters or elements in a scene.
- **Dialogue**: Dialogue in Theatre.js is a way for characters to communicate with each other. It can be used to advance the story or provide information to the user.
- **Animation**: Animation in Theatre.js is a way to add movement and life to your scenes. It can be used to move characters, change scene properties, and more.

## First Script: "Hello, Theatre!"

Now that we understand the core concepts, let's write our first Theatre.js script. We'll create a simple scene with one character who says "Hello, Theatre!".

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene
const scene = new Theatre.Scene();

// Create a character
const character = new Theatre.Character('Character');

// Add the character to the scene
scene.add(character);

// Make the character say "Hello, Theatre!"
character.say('Hello, Theatre!');
```

To run this script, save it as `helloTheatre.js` and run it using Node.js: `node helloTheatre.js`.

## Basic Structure of a Theatre.js Application

A typical Theatre.js application consists of several scenes, each with its own characters, dialogues, and animations. Here's a basic structure of a Theatre.js application:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create scenes
const scene1 = new Theatre.Scene();
const scene2 = new Theatre.Scene();

// Create characters
const character1 = new Theatre.Character('Character 1');
const character2 = new Theatre.Character('Character 2');

// Add characters to scenes
scene1.add(character1);
scene2.add(character2);

// Write dialogues and animations
character1.say('Hello, Theatre!');
character2.move({ x: 100, y: 200 });
```

In the next chapter, we'll dive deeper into scenes and learn how to add elements and control their properties. Stay tuned!

[Next Chapter: Working with Scenes](chapter3-scenes.md)
