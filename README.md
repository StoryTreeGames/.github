<div align="center">
  <img src="https://github.com/StoryTreeGames/StoryTreeGames/blob/main/StoryTree_Cropped.png" />
</div>

A fully open source game engine written in Zig. The idea is to create libraries in pure Zig that can create windows, render with "native" APIs, access system resources, etc...


**Goals**

- Cross Platform: Windows, Linux, Macos, Web, Android, IOS
- Use zig libraries that already exist that fit all following goals
- Minimal `C` dependencies
- Well maintained
- Uses Zig's potential

The minimal `C` dependencies goal is to push the game engine away from the current popular C paradigms. Zig is compatible with C, but it can do so much better. If most of the engine and libraries where wrappers around C libraries why not just write the engine in the latest versions of `C++`? The engine may use some light wrappers around libraries like [`Dawn`](https://github.com/zig-gamedev/dawn) to get WebGPU functionality working, using [`zgpu`](https://github.com/zig-gamedev/zig-gamedev/tree/main/libs/zgpu). However, if a pure Zig implementation exists and the only C dependencies are with the `Vulkan`, `DirectX`, and `Metal` APIs then that will be used instead. If no project or library exists that fit the minimal `C` requirement then a new project/library will be created to fit this.

Minimal `C` Exceptions:

- Operating System APIs
- Implmentation APIs that are in C and are too complex to convert to Zig
  - ex: [`zgpu`](https://github.com/zig-gamedev/zig-gamedev/tree/main/libs/zgpu)  

> [!NOTE]
> - This project is currently just a bunch of brainstorming and is only maintained by a single developer.
> - The core developer is not an expert in Zig and is using this project as a learning tool
> - Contributions and ideas are more than welcome. See the [discussions]([https://github.com/StoryTreeGames/StoryTreeGames/issues](https://github.com/orgs/StoryTreeGames/discussions)) section for what is needed, areas that need work, and how to contribute.

## Libraries
- Windowing: All functionality around cross platform windows, window events, and anything related to windows/apps
- Audio: A cross platform library for playing and manipulating audio
- Font: A cross platform api for reading font data
- ECS: Entity component system
- Render: Rendering api using WebGPU standards that can be used accross Windows, Macos, Linux, Web, Android, and IOS
- Engine: Combination of all libraries to make a simple and easy to use API to load and manage resources, render entities, and handle events
- more ...

## Inspiration

- [`Mach`](https://machengine.org/)
  - [github](https://github.com/hexops/mach/tree/main)
- [`Evie Engine`](https://github.com/DanWillans/Evie)
  - [Let's write an ECS](https://youtube.com/playlist?list=PLMClevbUJi9DsmIuij4RzjJ_kUyrQufEs&si=_NJz-DaHthcH9CI4)
- [`fontaine`](https://github.com/ziglibs/fontaine)
- [`zig-miniaudio`](https://github.com/prime31/zig-miniaudio)
- [`zig-wav`](https://github.com/dbandstra/zig-wav)
- [`zua`](https://github.com/squeek502/zua)
- [`zig-sparse-set`](https://github.com/Srekel/zig-sparse-set)
- [`zig-vulkan-triangle`](https://github.com/andrewrk/zig-vulkan-triangle)

- [`awesome-zig`](https://github.com/nrdmn/awesome-zig)
- [`zig-gamedev`](https://github.com/zig-gamedev/zig-gamedev)
