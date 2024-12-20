This program is a C++ implementation that uses OpenGL to render a 3D scene featuring models like Batman, Joker, Batmobile, and a bat. The scene includes a skybox that provides a "Gotham nights" environment. Here's a summary of the code:

Libraries Used
GLAD: For managing OpenGL function pointers.
GLFW: For window management and input handling.
STB_IMAGE: For loading textures.
GLM: For mathematics operations like transformations (matrices, vectors).
Custom Shader, Camera, and Model Classes: For managing OpenGL shaders, camera movement, and loading 3D models.
Key Features of the Program
Window Setup

Creates a window using GLFW with OpenGL 3.3 Core profile.
Configures the window to capture the mouse for a first-person camera experience.
Camera

A Camera class is used to manage first-person navigation.
Supports mouse movement, scroll, and keyboard inputs for controlling the camera position and direction.
Skybox

A skybox is created using cube-mapped textures to render a Gotham city background.
The cubemap uses six images for the environment (right, left, top, bottom, front, back).
3D Models

Loads 3D models such as Batman, Joker, Batmobile, and a bat using a custom Model class.
Positions and animates models in the scene:
The bat rotates dynamically.
The Batmobile and Joker have simple animations.
Shaders

Two shaders are used:
One for rendering the 3D models.
Another for rendering the skybox.
Rendering Pipeline

Depth testing is enabled for proper rendering order.
Each frame:
Clears the screen.
Updates the camera and model positions.
Draws the models and skybox.
Uses matrices (view, projection, model) to manage transformations like scaling, rotation, and translation.
Keyboard Controls
W, A, S, D: Move the camera forward, left, backward, and right.
ESC: Close the window.
Mouse and Scroll
Mouse Movement: Adjusts the camera direction.
Scroll Wheel: Zooms in or out by adjusting the camera's field of view.
Observations
The code animates models and gives a dynamic feel to the scene.
Models are loaded using .obj files with textures for realism.
The skybox enhances the visual environment by providing a night-time Gotham City look.

https://www.youtube.com/watch?v=GklmYtJTelE
