# UE4-Delaunay-Triangulation
Unreal Engine 4 Delaunay Triangulation **Module**

![](https://s3.bmp.ovh/imgs/2021/11/44a9294ad2134636.png)

### 1. What Is *Delaunay Triangulation*

[Link](https://www.bilibili.com/read/cv9358144)



### 2. Create Custom Module

You need to know how to add custom modules in UE4.



### 3. *Delaunay Triangulation* In UE4

First, [this repository](https://github.com/Jay2645/Unreal-Polygonal-Map-Gen) contains the *Delaunator* module in `Source/Delaunator` directory. You can directly put it in your own project. To be specific,

1. Clone  [this repository](https://github.com/Jay2645/Unreal-Polygonal-Map-Gen).
2. Add custom module `Source/Delaunator` in your project.



Plus, you have to **make some modifications** to the source file. Otherwise, errors would occur during compilation. Specifically,

- `#include "ModuleManager.h"` → `#include "Modules/ModuleManager.h"`
- `#include "GenericPlatform.h"` → `#include "GenericPlatform/GenericPlatform.h"`
- Whenever function `UE_LOG` occurs, include `Delaunator.h` in the cpp file.
- Delete `Test` directory directly. Otherwise you will spend some time debugging.

Now, you can use *Delaunay Triangulation* in your UE4 project.



### Notice

The code in my repository is the *Delaunay Triangulation* after my modification, based on my environment. Therefore, you may use it directly.

> **My UE4 Version: 4.27**

