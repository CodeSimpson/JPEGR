## 1. JPEG如何保存

JPEG图片格式组成为：

粗体为JPEG组成中的必须部分。

| 名称       | 标记码 | 含义         |
| :------- | :-- | :--------- |
| **SOI**  |     | 文件头        |
| **APP0** |     | 图像识别信息     |
| **DQT**  |     | 定义量化表      |
| **SOF0** |     | 图像基本信息     |
| **DHT**  |     | 定义Huffman表 |
| DRI      |     | 定义重新开始间隔   |
| **SOS**  |     | 扫描行开始      |
| **EOI**  |     | 文件尾        |

### 1.1 Android如何识别JPEG文件？

原理非常简单，通过判断jpeg二进制文件的前3个字节是否是以**FF D8 FF**开始，如果是就认为它是JPEG图。

### 1.2 JPEG文件的段结构





> 参考: <https://blog.csdn.net/huabiaochen/article/details/108044123>

