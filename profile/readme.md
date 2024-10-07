<div align="center">
  <img src="https://github.com/StoryTreeGames/StoryTreeGames/blob/main/StoryTree_Cropped.png" />
</div>

A fully open source game engine written in Zig. The idea is to create "from scratch" libraries that can create windows, render with "native" APIs, access system resources, etc...

> Note: This project is currently just a bunch of brainstorming and is only maintained by a single developer. Contributions and ideas are more than welcome. See the [discussions]([https://github.com/StoryTreeGames/StoryTreeGames/issues](https://github.com/orgs/StoryTreeGames/discussions)) section for what is needed, areas that need work, and how to contribute.

## Libraries
- [ ] Sys: System API access cross platform
- [ ] Audio: A cross platform library for playing and manipulating audio
- [ ] Font: A cross platform api for font data
- [ ] Render: A rendering engine that can render graphics and UI to a cross platform window/frame
  - Custom or Sourced WebGPU implementation
- [ ] Engine: Game engine specific structures and systems

### Sys

  - [ ] Windowing
  - [ ] Sys calls
  - [ ] IO Events
  - [ ] Linux, Macos, Windows, Web (WASM), Android, IOS
        
### Audio

  - [ ] Reads multiple formats
  - [ ] Streams data with timestamps and audio information
        
### Font

  - [ ] Reads multiple formats
  - [ ] Supports font fallback
  - [ ] Agnostic data that can be transformed 

### Engine

  - [ ] Cross Compile
  - [ ] Entity Component System
  - [ ] Scripting: Allows for scripting in multiple different languages
  - [ ] GUI ? (long term)

## Inspiration

- [`Mach`](https://machengine.org/)
  - [github](https://github.com/hexops/mach/tree/main)
- [`Evie Engine`](https://github.com/DanWillans/Evie)
  - [Let's write an ECS](https://youtube.com/playlist?list=PLMClevbUJi9DsmIuij4RzjJ_kUyrQufEs&si=_NJz-DaHthcH9CI4) 
