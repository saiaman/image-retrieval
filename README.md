## 图像检索

开始整理这两三年自己在image retrieval的一些资料，方便来年的毕业设计。

| 单词数目 | SIFT or rootSIFT | 空间校正与否 | 重排深度 | 检索精度mAP | 查询时间(55张)(s) |
| ---------|:----------------:| :-----------:|:--------:|:-----------:|:-----------------:|
|   500k   |    rootSIFT      |      否      |     -    |    74.82%   |       5.345534    |
|   500k   |    rootSIFT      |      是      |     1    |    74.82%   |      19.176519    |
|   500k   |    rootSIFT      |      是      |    20    |    77.77%   |      21.646773    |
|   500k   |    rootSIFT      |      是      |    30    |    79.06%   |      21.615220    |
|   500k   |    rootSIFT      |      是      |    40    |    79.86%   |      23.453462    |
|   500k   |    rootSIFT      |      是      |    50    |    80.54%   |      23.588034    |
|   500k   |    rootSIFT      |      是      |    100   |    82.18%   |      24.942057    |

**查询时间**：查询时间是单词查询的结果，并没有进行多次查询进行平均，此外查询时间是查询和计算mAP时间的总和。

### 基于SIFT特征点匹配

[SIFT on GPU (SiftGPU)](http://ccwu.me/), works for nVidia, ATI and Intel cards..
