# Dataset A: UAV Aerial Person Detection Dataset（数据集A：无人机航拍人体检测数据集）

## Overview | 简介

**EN**: Dataset A is a self-constructed UAV aerial dataset for single-class (person) object detection, used for model training, component contribution analysis, and model comparison. It contains 2,283 UAV aerial images at 800×800 resolution with 8,367 person annotations. Under 640×640 input resolution, 97.04% of targets are smaller than 32×32 pixels, making it a typical representative of complex search-and-rescue (SAR) scenes with numerous occluded samples.

**中文**：数据集A为自研无人机航拍数据集，面向单类（person）目标检测任务，用于模型训练、成分贡献分析和模型比较。数据集包含2283张800×800分辨率的航拍图像，共8367个人体目标标注。640×640输入尺寸下小于32×32像素的小目标占比达97.04%，存在大量目标遮挡样本，是复杂搜救（SAR）场景的典型代表。

## Statistics | 数据统计

- Total images | 图像总数: 2,283 (800×800)
- Person annotations | 人体目标标注: 8,367 (single class: person | 单类：person)
- Small targets (<32×32 px @ 640×640 input) | 小目标占比: 97.04%
- Split | 划分: train 1,595 / val 458 / test 230 (7:2:1)
- Scenes | 场景: highway, urban, forest, lake, snow | 公路、城市、森林、湖泊、雪地
- Disturbances | 干扰: rain, fog, strong light, low light, Gaussian noise | 雨、雾、强光、暗光、高斯噪声

## Collection | 数据采集

**EN**: Images were captured by a DJI Flip UAV and extracted from aerial video, with flight altitudes concentrated at 65–80 m and 100–120 m.

**中文**：图像由大疆 Flip 无人机拍摄视频抽帧获取，飞行高度集中在65–80米、100–120米。

## Annotation Format | 标注格式

**EN**: Annotations follow the YOLO format: one `.txt` file per image, single class `person` (class_id = 0). Note: this repository releases **images only**; annotations are available upon reasonable request (contact: wangguoxu@sylu.edu.cn).

**中文**：标注采用 YOLO 格式，每张图像对应一个 `.txt` 标签文件，单类 `person`（class_id = 0）。注意：本仓库仅发布图像，标注可通过合理申请联系作者获取（联系方式：wangguoxu@sylu.edu.cn）。

## Dataset Structure | 目录结构

```
images/
├── train/  # A1.jpg – A1595.jpg
├── val/    # A1596.jpg – A2053.jpg
└── test/   # A2054.jpg – A2283.jpg
```

## Intended Use | 用途说明

**EN**: This dataset is released for academic research only.

**中文**：本数据集仅用于学术研究。

## License | 许可证

**EN**: This dataset is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) (Attribution-NonCommercial 4.0 International). You are free to use, share, and adapt this dataset for non-commercial purposes, provided that appropriate attribution is given. See the [LICENSE](LICENSE) file for the full license text.

**中文**：本数据集采用 [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)（署名-非商业性使用 4.0 国际）许可协议发布。任何人可在非商业目的下自由使用、共享和修改本数据集，但须注明来源与作者。完整许可文本见 [LICENSE](LICENSE) 文件。

## Citation | 引用

[待论文录用后填写 BibTeX]

## Authors & Contact | 作者与联系方式

**EN**: Authors: Wenbo Chang, Guoxu Wang, Umar Yahya

Corresponding author: Guoxu Wang (wangguoxu@sylu.edu.cn)

**中文**：作者：Wenbo Chang、Guoxu Wang、Umar Yahya

通讯作者：Guoxu Wang（wangguoxu@sylu.edu.cn）
