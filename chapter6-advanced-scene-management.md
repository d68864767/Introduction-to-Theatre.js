# Chapter 6: Advanced Scene Management

Welcome to the sixth chapter of our comprehensive guide to Theatre.js! In this chapter, we will explore advanced scene management techniques, including nested scenes, dynamic scene creation and deletion, and scene lifecycle and hooks.

## Nested Scenes

In Theatre.js, you can create nested scenes, which are scenes within scenes. This can be useful for creating complex applications with multiple layers of interaction. Here's how you can create a nested scene:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene
const scene = new Theatre.Scene();

// Create a nested scene
const nestedScene = new Theatre.Scene();

// Add the nested scene to the parent scene
scene.add(nestedScene);
```

## Dynamic Scene Creation and Deletion

Theatre.js allows you to dynamically create and delete scenes at runtime. This can be useful for creating dynamic applications where scenes change based on user input or other factors. Here's how you can dynamically create and delete scenes:

```javascript
// Dynamically create a scene
const dynamicScene = new Theatre.Scene();

// Add the dynamic scene to the parent scene
scene.add(dynamicScene);

// Dynamically delete a scene
scene.remove(dynamicScene);
```

## Scene Lifecycle and Hooks

Every scene in Theatre.js goes through a lifecycle, which includes creation, update, and deletion. You can hook into these lifecycle events to run custom code at specific points in the scene's lifecycle. Here's how you can use scene lifecycle hooks:

```javascript
// Hook into the scene's creation event
scene.on('create', () => {
  console.log('Scene created!');
});

// Hook into the scene's update event
scene.on('update', () => {
  console.log('Scene updated!');
});

// Hook into the scene's deletion event
scene.on('delete', () => {
  console.log('Scene deleted!');
});
```

In the next chapter, we'll dive into complex character control, including custom character behaviors, interaction with user input, and character motion and pathfinding. Stay tuned!

[Next Chapter: Complex Character Control](chapter7-complex-character-control.md)
