# astc-encoder

ASTC（Adaptive Scalable Texture Compression）是由ARM和AMD联合开发的一种先进的纹理压缩技术。它已经被采纳为OpenGL和OpenGL ES API的官方Khronos扩展，并作为Vulkan API的一个标准可选功能。
ASTC Encoder（Adaptive Scalable Texture Compression Encoder）是ARM推出的一款使用ASTC纹理压缩标准对图像进行压缩和解压的参考代码。

## 目录结构

```
Docs             #文档
Source           #源代码
Test             #测试代码
Utils            #特定场景配置测试代码
jenkins          #构建脚本
CMakeLists.txt   #编译描述文件
LICENSE.txt      #版权声明
README.md        #软件说明
```

## 引入目的

OpenHarmony上引入ASTC主要用于图库缩略图和其他应用预置图的压缩。ASTC码流可以直接由GPU解码显示，降低传输数据量和CPU解码耗时。

## OpenHarmony对于astc-encoder的适配

astc-encoder编译框架时编译，使用BUILD.gn进行配置编译。
基于OpenHarmony的需求，astc-encoder提供的能力：
- GPU支持的ASTC纹理压缩码流的编码

## OpenHarmony使用方法

提供生成ASTC码流的能力，码流可以直接由GPU解码显示


