# Nanshan Street View Segmentation Results

南山区研究区 7,636 张街景的语义分割与窗墙比结果。

## 数据内容

- 7,636 张 512×512 单通道 PNG 分割掩膜
- 类别：0 = background，1 = wall，2 = window or door
- 逐图 WWR 表与 JSONL
- 采样点、80 m 网格和建筑尺度 WWR 表及 GeoPackage
- WWR 定义：`window_pixels / (wall_pixels + window_pixels)`

数据压缩包位于仓库的 **Releases** 页面；`MANIFEST.csv` 提供每个文件的相对路径、字节数和 SHA-256。

## 目录结构

```text
data/
├── masks/<point_id>/*_mask.png
└── tables/
    ├── wwr_predictions.csv
    ├── sample_points_wwr.csv
    ├── grid_80m_wwr.csv
    └── buildings_grid_wwr.csv
```

仓库仅包含结果数据，不包含模型权重、API 密钥、访问令牌或运行日志。

