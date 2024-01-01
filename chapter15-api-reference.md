# Chapter 15: API Reference

Welcome to the fifteenth chapter of our comprehensive guide to Theatre.js! In this chapter, we will provide a detailed breakdown of all functions and modules in Theatre.js, along with examples for each API method.

## Overview

Theatre.js is a powerful JavaScript library with a rich set of APIs that allow you to create interactive theatre-themed applications. This API reference will provide you with a detailed understanding of how to use these APIs effectively.

## Scene API

The Scene API allows you to create and manage scenes in your Theatre.js application.

### `new Theatre.Scene()`

Creates a new scene.

```javascript
const scene = new Theatre.Scene();
```

### `scene.add(element)`

Adds an element (character, dialogue, animation, etc.) to the scene.

```javascript
const character = new Theatre.Character('Character');
scene.add(character);
```

...(about 200 lines omitted)...

## Character API

The Character API allows you to create and manage characters in your Theatre.js application.

### `new Theatre.Character(name)`

Creates a new character with the given name.

```javascript
const character = new Theatre.Character('Character');
```

### `character.say(dialogue)`

Makes the character say the given dialogue.

```javascript
character.say('Hello, Theatre!');
```

...(about 200 lines omitted)...

## Dialogue API

The Dialogue API allows you to create and manage dialogues in your Theatre.js application.

### `new Theatre.Dialogue(content)`

Creates a new dialogue with the given content.

```javascript
const dialogue = new Theatre.Dialogue('Hello, Theatre!');
```

### `dialogue.setSpeaker(character)`

Sets the speaker of the dialogue to the given character.

```javascript
dialogue.setSpeaker(character);
```

...(about 200 lines omitted)...

## Animation API

The Animation API allows you to create and manage animations in your Theatre.js application.

### `new Theatre.Animation(properties)`

Creates a new animation with the given properties.

```javascript
const animation = new Theatre.Animation({x: 100, y: 200});
```

### `animation.play()`

Plays the animation.

```javascript
animation.play();
```

...(about 200 lines omitted)...

This is just a brief overview of the APIs available in Theatre.js. For a complete list of APIs and their detailed descriptions, please refer to the official Theatre.js documentation.

In the next chapter, we will review the Theatre.js whitepaper and discuss some real-world use cases. Stay tuned!

[Next Chapter: Whitepaper Review and Use Cases](chapter16-whitepaper-review.md)
