# Cheeky First Person Controller

This project is a deliberately barebones first person controller for Unreal Engine 4, intended as a jumping off point for any first person projects I might pursue in future - and maybe it will help someone else do the same. I have kept things as modular as possible, so it should be straightforward to migrate some elements into existing projects.

Why 'Cheeky'? Well, it seemed funny prefixing all the classes with Cheeky. That's it.

[You can see a short demonstration video here.](https://www.youtube.com/watch?v=oIJvjmunHZY&feature=youtu.be)

## Features
- First Person Movement with multiple movement speeds and modifiers (e.g. moving backwards or side to side is slower)
- Interaction framework including messages, hold-style interactions, and movement/view restrictions
- Leaning system with collision detection
- Smooth stance system for standing, crouched, and prone
- Correct implementation of mouse smoothing that avoids using a spring arm (please stop doing this)
- Smooth, curve-driven headbob system, with a dynamic spring for vertical jump/landing
- Quake style camera roll (side to side)
- Dynamic DOF
- Basic footstep implementation (easily expandable!) synced with headbob
- Basic health component including fall damage calculation

## Things I might add
- A proper settings solution using a save binary file
- Parkour actions (climbing, vaulting)

## Getting Started
This project is 100% Blueprints, using Unreal Engine 4.25. No other pre-requisites required.

I have tried to stick to [Allar's fantastic style guide](https://github.com/Allar/ue4-style-guide), at least where it comes to asset naming conventions.

As this is still under active development / tinkering, relying on this for any project *right now* could be a bad idea. If you want to use it, I would recommend creating your character as a child blueprint of `BP_CheekyCharacter` so any changes upstream do not affect your own functionality.

## Contributing, Bug Reports, and Feature Requests
I can't imagine anyone wanting to contribute - but if you do, best to reach out to me on Discord: DaveFace#6969

If you encounter any problems, or want to request I add something (no guarantees!) please create a Github issue and I will look into it.

## Update History
**01/11/2020** : First Release

**01/11/2020** : Added more comments to code / classes. Cleaned up some classes (removed unused vars etc). Added crouch and run toggles. Added regenerating health option.

**02/11/2020** : Added basic interaction system

**03/11/2020** : Replaced simple crouch with a 3-way stance system on request

**06/11/2020** : Modified OnLanded event to reduce dependency on health component. Added framework for Parkour actions - doesn't actually do anything yet. Added several features to interactions including messages, hold interaction type, and primary/secondary interaction events. Added some more example interactors including a fancy door. Added a basic level/blueprint communication system.

## Authors

* **Dave Watts** - [ArtStation](https://www.artstation.com/daveface) / [Twitter](https://twitter.com/therealdaveface)

## License

This project is licensed under the MIT License. Some example content (see acknowledgements) is not included in this license.

## Acknowledgments

- Example footstep sounds from https://freesound.org/
