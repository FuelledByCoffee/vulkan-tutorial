# Ottocento Engine

![screenshot_sandoy_model.jpg](src%2Fmodels%2Fscreenshot_sandoy_model.jpg)

This is a study project that initially follows the 
[Vulkan Implementation Tutorial](https://vulkan-tutorial.com/). 
The idea here is to solely
document the process and make it easier for me to further
reference the code inside the tutorial. 
The end goal, however, is to be able to expand this project, based on the Vulkan Tutorial to create my own
Architectural BIM Engine.
The idea is also help other Vulkan users to implement the features covered in this repository.

I will be following the tutorial but will also make changes that suit my personal code style as well as
some other needs I will have to learn in the long run and want to implement on other projects. 
For this reason, the code on this project won't be a 100% copy of the original code from the Vulkan Tutorial.
If you want to see the original code, please reference it on the `References` section.

Additionally, I will be adding lots of comment lines — sometimes more than "strictly necessary" — for studying purposes. 
Sometimes the lines are just a copy of the explanations inside the Vulkan-Tutorial, sometimes they are personal notations
for me to remember later and make it easier to implement in other projects. This is a study project after all.

### What is Vulkan?
> Vulkan is a new API by the Khronos group (known for OpenGL) that provides a much better 
abstraction of modern graphics cards. This new interface allows you to better describe what your 
application intends to do, which can lead to better performance and less surprising driver behavior 
compared to existing APIs like OpenGL and Direct3D. The ideas behind Vulkan are similar to those of 
Direct3D 12 and Metal, but Vulkan has the advantage of being fully cross-platform and allows you to develop 
for Windows, 
Linux and Android at the same time.
> 

### Documentation

- To see how to build the project, please refer to the [Build Guide](./doc/build.md)
- To see how we style our code, please refer to the [Code Style Guide](./doc/styleguide.md).


### Additional (not covered inside the vulkan-tutorial)
- [x] Setting up Development Environment with Premake5.lua for Windows and Linux.
- [x] UI: Win32 Dark Titlebar to follow the Darkmode from the system.
- [x] GLFW: Change the Window Icon (further can be expanded to be a call to the GPU to decode a Hex Array).
- [x] Camera: WASD navigation with Right mouse button.
- [x] Camera: Orbit around object with full axis freedom and no gimble lock (quartenion rotation).
- [x] Camera: Front, Right, Top and Isonometric views based on Blender's camera hotkeys for user integration.
- [x] Infinite grid implementation with an independent DescriptorSet, Graphics Pipeline, Vertex and Fragment Shaders.
- [x] Smooth Resizing.
- [ ] Integrate Vulkan with Immediate mode GUI.
- [ ] Lighting and illumination.
- [ ] Create a single command buffer (`setupCommandBuffer`) to execute them asynchronously for higher throughput.

### Steps from Vulkan Tutorial
- [x] Setting up Development Environment.
- [x] Instance Creation.
- [x] Validation Layers Implementation.
- [x] Physical Devices and Queue Families selection.
- [x] Logical device and queues.
- [x] Window Surface creation.
- [x] Swap Chain
- [x] Image Views
- [x] Graphics Pipeline Basics
  - [x] Shader Modules
  - [x] Fixed Functions
  - [x] Render Passes
- [x] Frame buffers
- [x] Command Buffers
- [x] Rendering and Presentation (finally rendering the first triangle)
- [x] Frames in flight
- [x] Swap Chain Recreation
- [X] Vertex Buffers
- [x] Uniform Buffers
- [x] Texture Mapping
  - [x] Images
  - [x] Image view and sampler
  - [x] Combined Image Sampler
- [x] Depth Buffering
- [x] Loading Models
- [x] Generating Mipmaps
- [x] Multisampling

### References/Resources
- [Vulkan Tutorial](https://vulkan-tutorial.com/)
- [Learn Vulkan Wiki](https://github.com/PAMinerva/LearnVulkan/wiki/01.B-Hello-Triangle)
- [Vulkanised 2024: Common Mistakes When Learning Vulkan - Charles Giessen](https://www.youtube.com/watch?v=0OqJtPnkfC8)
- [Rasterizer Algorithm Explanation](https://www.youtube.com/watch?v=t7Ztio8cwqM)
- [Homogeneous Coordinates](https://en.wikipedia.org/wiki/Homogeneous_coordinates)
- [OpenGL Tutorial: Matrices](https://www.opengl-tutorial.org/beginners-tutorials/tutorial-3-matrices/)
- [Simple "Infinite" Grid Shader](https://dev.to/javiersalcedopuyo/simple-infinite-grid-shader-5fah)
- [An introduction to shader derivative functions](https://www.aclockworkberry.com/shader-derivative-functions/)
- [The Best Darn Grid Shader (Yet)](https://bgolus.medium.com/the-best-darn-grid-shader-yet-727f9278b9d8#1d80)
- [Apodaca, Anthony A., and Larry Gritz, eds. 1999. Advanced RenderMan: Creating CGI for Motion Pictures.](https://books.google.com.br/books?id=6_4VaJiOx7EC&q=Pulsetrain&redir_esc=y#v=onepage&q&f=false)
- [Entity Component System FAQ](https://github.com/SanderMertens/ecs-faq)
- [Anti-Aliased Grid Shader](https://madebyevan.com/shaders/grid/)
- [How to (and how not to) fix color banding](https://blog.frost.kiwi/GLSL-noise-and-radial-gradient/)
- [Using Arrays of Textures in Vulkan Shaders](https://kylehalladay.com/blog/tutorial/vulkan/2018/01/28/Textue-Arrays-Vulkan.html)
- [How not to test graphics algorithms](https://bartwronski.com/2019/08/14/how-not-to-test-graphics-algorithms/)

### License
Ottocento Engine is licensed under the GNU General Public License, Version 3.
See License