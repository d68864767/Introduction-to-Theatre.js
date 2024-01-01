# Chapter 9: State Management in Theatre.js

Welcome to the ninth chapter of our comprehensive guide to Theatre.js! In this chapter, we will explore state management in Theatre.js, learn how to share state across scenes, and understand reactive state changes.

## Introduction to State Management

In Theatre.js, state management is a crucial part of creating interactive applications. The state of an application refers to the data that changes over time and affects the behavior of the application. For example, the state could include the current scene, the position of a character, or the dialogue that is currently being displayed.

State management in Theatre.js is handled through a combination of JavaScript's built-in state management features and Theatre.js's own state management tools. Let's take a closer look at how this works.

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene
const scene = new Theatre.Scene();

// Define the initial state
const initialState = {
  currentScene: 'home',
  characterPosition: { x: 0, y: 0 },
  currentDialogue: ''
};

// Create a state object
const state = new Theatre.State(initialState);

// Access the state
console.log(state.get('currentScene')); // 'home'
```

## Sharing State Across Scenes

One of the powerful features of Theatre.js is the ability to share state across multiple scenes. This allows you to create complex applications where actions in one scene can affect the state of another scene.

Here's an example of how you can share state across scenes:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create two scenes
const scene1 = new Theatre.Scene();
const scene2 = new Theatre.Scene();

// Define the initial state
const initialState = {
  currentScene: 'home',
  characterPosition: { x: 0, y: 0 },
  currentDialogue: ''
};

// Create a state object
const state = new Theatre.State(initialState);

// Share the state across scenes
scene1.state = state;
scene2.state = state;

// Change the state in scene1
scene1.state.set('currentScene', 'scene1');

// Access the state in scene2
console.log(scene2.state.get('currentScene')); // 'scene1'
```

## Reactive State Changes

Theatre.js also supports reactive state changes, which means that you can set up your application to automatically respond to changes in the state. This is done using the `watch` method, which allows you to specify a function that will be called whenever a specific part of the state changes.

Here's an example of how you can set up reactive state changes:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene
const scene = new Theatre.Scene();

// Define the initial state
const initialState = {
  currentScene: 'home',
  characterPosition: { x: 0, y: 0 },
  currentDialogue: ''
};

// Create a state object
const state = new Theatre.State(initialState);

// Set up a watcher for the 'currentScene' property
state.watch('currentScene', (newValue, oldValue) => {
  console.log(`The current scene has changed from ${oldValue} to ${newValue}`);
});

// Change the 'currentScene' property
state.set('currentScene', 'scene1'); // Logs: "The current scene has changed from home to scene1"
```

In the next chapter, we'll dive into creating custom plugins for Theatre.js. Stay tuned!

[Next Chapter: Custom Plugins for Theatre.js](chapter10-custom-plugins.md)
