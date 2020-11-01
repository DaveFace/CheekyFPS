# Cheeky First Person Controller

This project is a deliberately barebones first person controller for Unreal Engine 4, intended as a jumping off point for any first person projects I might pursue in future - and maybe it will help someone else do the same. I have kept things as modular as possible, so it should be straightforward to migrate some elements into existing projects.

Why 'Cheeky'? Well, it seemed funny prefixing all the classes with Cheeky. That's it.

[You can see a short demonstration video here.](https://www.youtube.com/watch?v=oIJvjmunHZY&feature=youtu.be)

## Features
- First Person Movement with multiple movement speeds and modifiers (e.g. moving backwards or side to side is slower)
- Leaning system with collision detection
- Smooth crouching
- Correct implementation of mouse smoothing that avoids using a spring arm (please stop doing this)
- Smooth, curve-driven headbob system, with a dynamic spring for vertical jump/landing
- Quake style camera roll (side to side)
- Dynamic DOF
- Basic footstep implementation (easily expandable!) synced with headbob
- Basic health component including fall damage calculation

## Things I might add
- A proper settings solution using a save binary file
- Some kind of interaction system

## Getting Started
This project is 100% Blueprints, using Unreal Engine 4.25. No other pre-requisites required.

I have tried to stick to [Allar's fantastic style guide](https://github.com/Allar/ue4-style-guide), at least where it comes to asset naming conventions.

## Update History
**01/11/2020** : First Release
**01/11/2020** : Added more comments to code / classes. Cleaned up some classes (removed unused vars etc). Added crouch and run toggles. Added regenerating health option.

## Contributing or Feature Requests
I can't imagine anyone wanting to contribute - but if you do, best to reach out to me on Discord: DaveFace#6969

Also happy to take feature requests within reason, if I think it could be something cool to add.

## Authors

* **Dave Watts** - [ArtStation](https://www.artstation.com/daveface) / [Twitter](https://twitter.com/therealdaveface)

## License

This project is licensed under the MIT License. Some example content (see acknowledgements) is not included in this license.

## Acknowledgments

- Example footstep sounds from https://freesound.org/
