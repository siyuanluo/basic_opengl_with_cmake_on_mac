# basic_opengl_with_cmake_on_mac
Basic environment to make OpenGL works on MacOS with Cmake( in VSCode ) 



1. Firstly, you should download GLFW/glad files and put them in your system *include/* and *lib/* folder. ( */usr/local/...* )
[Reference](https://learnopengl.com/Getting-started/Creating-a-window)

2. If you use VSCode, you should first download the Extension:

   **C/C++ Entension Pack** / **CMake** / **CMake Tools** / **CMake Integration** / **CodeLLDB**

3. After doing those, just clone this repo, and open it. Run it on Terminal like this below:

   ~~~ bash
   mkdir build
   cd build
   cmake .. && make
   ./opengl_test
   ~~~

4. Then, you can draw two triangles on your windows.
