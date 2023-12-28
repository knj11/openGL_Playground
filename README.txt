pre: git clone --recursive "http link"
1) Open developer x64 tool set cmd prompt
- Windows Button -> All Apps -> Visual Studio Folder -> x64 Native Tools Command Prompt Visual Studio 2022
2) cd to root of project
3) mkdir build
4) run "cmake cmake -S . -B build -G "NMake Makefiles"
5) cmake --build build
6) build\space_invaders.exe

Main Learning Resource
https://learnopengl.com/Introduction

Open GL documentation
https://registry.khronos.org/OpenGL/specs/gl/glspec33.core.pdf

Standard Image loader
https://github.com/nothings/stb/tree/master

OpenGL Mathematics
https://github.com/g-truc/glm/tree/master