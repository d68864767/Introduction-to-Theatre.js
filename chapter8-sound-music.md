# Chapter 8: Sound and Music Integration

Welcome to the eighth chapter of our comprehensive guide to Theatre.js! In this chapter, we will learn how to integrate sound and music into our Theatre.js applications.

## Adding Background Music

Background music can greatly enhance the atmosphere and immersion of your theatre-themed applications. Here's how you can add background music to a scene in Theatre.js:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene
const scene = new Theatre.Scene();

// Add background music to the scene
scene.addSound('backgroundMusic', 'path/to/your/music/file.mp3');
scene.playSound('backgroundMusic');
```

## Sound Effects for Actions

Sound effects can be used to provide auditory feedback for actions and events in your application. Here's how you can add a sound effect to a character's action:

```javascript
// Import the Theatre.js library
const Theatre = require('theatre');

// Create a new scene and a character
const scene = new Theatre.Scene();
const character = new Theatre.Character('Character');
scene.add(character);

// Add a sound effect to the character's action
character.addAction('jump', () => {
  // Action logic here...
  scene.playSound('jumpSound');
});
```

## Controlling Sound Playback

Theatre.js provides several methods for controlling sound playback. Here are some examples:

```javascript
// Play a sound
scene.playSound('backgroundMusic');

// Pause a sound
scene.pauseSound('backgroundMusic');

// Stop a sound
scene.stopSound('backgroundMusic');

// Loop a sound
scene.loopSound('backgroundMusic');
```

In the next chapter, we will dive into state management in Theatre.js, which is a crucial aspect of creating dynamic and interactive applications.

[Next Chapter: State Management in Theatre.js](chapter9-state-management.md)
