# Chapter 7: Complex Character Control

Welcome to the seventh chapter of our comprehensive guide to Theatre.js! In this chapter, we will delve into more complex aspects of character control, including custom character behaviors, interaction with user input, and character motion and pathfinding.

## Custom Character Behaviors

Characters in Theatre.js are not limited to predefined behaviors. You can create custom behaviors to make your characters more dynamic and interactive. Here's an example of how you can create a custom behavior:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a character
const character = new Theatre.Character('Character');

// Define a custom behavior
character.behavior('greet', function() {
  this.say('Hello, Theatre!');
});

// Use the custom behavior
character.greet();
```

In this example, we've defined a custom behavior called 'greet' that makes the character say "Hello, Theatre!". We can then use this behavior by calling `character.greet()`.

## Interaction with User Input

Theatre.js allows characters to interact with user input, making your applications more engaging and interactive. Here's an example of how you can make a character respond to a mouse click:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a character
const character = new Theatre.Character('Character');

// Make the character respond to a mouse click
character.on('click', function() {
  this.say('You clicked me!');
});
```

In this example, we've used the `on` method to make the character respond to a mouse click by saying "You clicked me!".

## Character Motion and Pathfinding

Theatre.js provides powerful features for character motion and pathfinding, allowing you to create complex movements and interactions. Here's an example of how you can make a character move along a path:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a character
const character = new Theatre.Character('Character');

// Define a path
const path = [
  { x: 0, y: 0 },
  { x: 100, y: 0 },
  { x: 100, y: 100 },
  { x: 0, y: 100 }
];

// Make the character move along the path
character.moveAlong(path);
```

In this example, we've defined a path as an array of coordinates and used the `moveAlong` method to make the character move along this path.

In the next chapter, we'll explore how to integrate sound and music into your Theatre.js applications. Stay tuned!

[Next Chapter: Sound and Music Integration](chapter8-sound-music.md)
