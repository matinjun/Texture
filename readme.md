# 纹理实验说明
## 对原本的数据结构更改
1. [mesh.h](./mesh.h)中修改了faceList的类型，由原来的float直接改成了vec3
2. [Mesh_Painter.cpp](./Mesh_Painter.cpp)文件不能简单的复制原来的实验4.1文件，需要做一些修改，建议直接copy
## 读取文件
1. 方法很多种，主要是针对fstream的使用，这里实现字符分割的方法是再多使用一个**char**型数据吃掉“/”就可以了，其余与std::cin类似
2. 需要定义物体的边界（以一个正方体为边界），中心，具体见实现
## main函数部分
主要注意下旋转速度，以及位置，具体见[main](Texture_Mapping.cpp)
