# astc-encoder

ASTC（Adaptive Scalable Texture Compression）是由Arm和AMD联合开发的一种先进的纹理压缩技术。它已经被采纳为OpenGL和OpenGL ES API的官方Khronos扩展，并作为Vulkan API的一个标准可选功能。
ASTC Encoder（Adaptive Scalable Texture Compression Encoder），则是Arm推出的一款使用ASTC纹理压缩标准进行压缩和解压图像的命令行工具。与2.5版本相比，3.x系列的主要目标是要保持图像质量不变或更好的前提下，进一步提高性能。

## 目录结构

```
Docs             #性能测试数据
Source           #源代码
Test             #测试代码
Utils            #特定场景配置测试代码
jenkins          #构建脚本
CMakeLists.txt   #编译描述文件
LICENSE.txt      #版权声明
README.md        #软件说明
```

## Openharmony对于astc-encoder的适配

astc-encoder编译框架时编译，使用BUILD.gn进行配置编译。
基于Openharmony的需求，astc-encoder提供的能力：
- GPU支持的ASTC纹理压缩码流的编码

## astc-encoder使用文档

有关完整astc-encoder的使用可参考：
https://github.com/ARM-software/astc-encoder
