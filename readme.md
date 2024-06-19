- Install gcc via scoop
- Download glfw and glew
- Genrerate GLAD
- Change the imports

```cpp
// change this
#include <glad/glad.h>

// to this (also in the glad.c)
#include "include/glad.h"
```

```sh
# runner
gcc main.cpp glad.c -lstdc++ -o main.exe -I ./include -I C:\\Users\\sabit\\glfw-3.4.bin.WIN64\\include -I C:\\Users\\sabit\\glew-2.1.0\\include -L C:\\Users\\sabit\\glfw-3.4.bin.WIN64\\lib-mingw-w64 -L C:\\Users\\sabit\\glew-2.1.0\\lib\\Release\\x64 -lglfw3dll -lglew32 -lopengl32
```