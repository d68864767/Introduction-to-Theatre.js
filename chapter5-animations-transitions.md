# Chapter 5: Animations and Transitions

Welcome to the fifth chapter of our comprehensive guide to Theatre.js! In this chapter, we will learn how to create animations, apply transition effects between scenes, and understand timing and sequencing of animations.

## Basic Animations

Animations are a powerful tool to bring your scenes to life. In Theatre.js, animations can be applied to any property of a scene or character. Here's how you can create a basic animation:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene
const scene = new Theatre.Scene();

// Create a character
const character = new Theatre.Character('Character');

// Add the character to the scene
scene.add(character);

// Create an animation
const animation = new Theatre.Animation({
  target: character,
  property: 'position',
  to: { x: 100, y: 100 },
  duration: 1000
});

// Start the animation
animation.start();
```

In this example, we create an animation that moves the character to the position (100, 100) over a duration of 1000 milliseconds.

## Transition Effects Between Scenes

Transition effects can be used to smoothly switch between different scenes. Here's how you can create a transition effect:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create two scenes
const scene1 = new Theatre.Scene();
const scene2 = new Theatre.Scene();

// Create a transition effect
const transition = new Theatre.Transition({
  from: scene1,
  to: scene2,
  duration: 1000
});

// Start the transition
transition.start();
```

In this example, we create a transition effect that switches from `scene1` to `scene2` over a duration of 1000 milliseconds.

## Timing and Sequencing Animations

Timing and sequencing are crucial for creating complex animations. Theatre.js provides several methods to control the timing and sequencing of animations. Here's an example:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene
const scene = new Theatre.Scene();

// Create a character
const character = new Theatre.Character('Character');

// Add the character to the scene
scene.add(character);

// Create two animations
const animation1 = new Theatre.Animation({
  target: character,
  property: 'position',
  to: { x: 100, y: 100 },
  duration: 1000
});
const animation2 = new Theatre.Animation({
  target: character,
  property: 'position',
  to: { x: 200, y: 200 },
  duration: 1000
});

// Sequence the animations
animation1.start().then(() => animation2.start());
```

In this example, `animation2` starts after `animation1` finishes.

In the next chapter, we'll dive into advanced scene management. Stay tuned!

[Next Chapter: Advanced Scene Management](chapter6-advanced-scene-management.md)
