# Chapter 3: Working with Scenes

Welcome to the third chapter of our comprehensive guide to Theatre.js! In this chapter, we will dive deeper into scenes, learn how to create them, understand their properties, and add elements to them.

## Creating Your First Scene

In Theatre.js, a scene is a container for all the elements that make up a part of your story. It can include characters, dialogues, animations, and more. Here's how you can create a scene:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene
const scene = new Theatre.Scene();
```

## Understanding Scene Properties

Each scene in Theatre.js has a set of properties that define its behavior and appearance. Here are some of the most important properties:

- **id**: A unique identifier for the scene.
- **width**: The width of the scene in pixels.
- **height**: The height of the scene in pixels.
- **background**: The background color or image of the scene.

You can access and modify these properties using the `get` and `set` methods:

```javascript
// Set the width and height of the scene
scene.set('width', 800);
scene.set('height', 600);

// Get the width and height of the scene
console.log(scene.get('width'));  // Outputs: 800
console.log(scene.get('height')); // Outputs: 600
```

## Adding Elements to a Scene

Once you've created a scene, you can add elements to it, such as characters, dialogues, and animations. Here's how you can add a character to a scene:

```javascript
// Create a character
const character = new Theatre.Character('Character');

// Add the character to the scene
scene.add(character);
```

You can add as many elements as you want to a scene, and they will be rendered in the order they were added.

In the next chapter, we'll learn about characters and dialogues, and how to control character interactions. Stay tuned!

[Next Chapter: Characters and Dialogues](chapter4-characters-dialogues.md)
