# StellarEraRes

StellarEra 的**资源与内容设计**仓库：概念图、图标、3D 模型，以及工厂玩法的内容框架。

## 目录

```
assets/
  icons/        图标（Pillow 绘制的占位图标 + Seedream 生成的高炉图标）
  concept/      高炉概念图、正交三视图、三视图拼版
  models/       Seed3D 生成并压缩后的高炉 GLB（约 6.5 MB，174,920 三角面，含 PBR 贴图）
design/
  planetary-factory-content.md   矿物/材料/部件/机器/行星发动机的内容设计稿
```

## 高炉素材

| 文件 | 来源 | 说明 |
| --- | --- | --- |
| `icons/furnace-ai.jpg` | Seedream 5.0 Pro | 1024×1024，等距视角图标 |
| `concept/furnace-concept.jpg` | Seedream 5.0 Pro | 概念图，作为三视图的参考图 |
| `concept/furnace-front.jpg` / `-side` / `-back` | Seedream 5.0 Pro | 白底正交三视图 |
| `concept/furnace-sheet.jpg` | 三图拼接 | 2304×768，3D 接口不接受该长宽比，仅作展示 |
| `models/furnace.glb` | Seed3D 2.0 + gltf-transform | 由图标生成；512 贴图、简化到 35%、量化后 6.5 MB |

`icons/iron-ore.png`、`coal.png`、`steel.png`、`furnace.png` 是用 Pillow 画的临时图标，用来先跑通 Nodeworks 里的资源容器与预览；`furnace-basecolor.png` 是手写 glTF 的原型贴图。

## 说明

- 图片与模型为 AI 生成，用于本项目内部原型；商用前请替换为已确认授权的素材。
- 生成用的 API Key 未写入仓库；请通过本地环境变量配置。
- 3D 预览可直接把 `models/furnace.glb` 拖进 Nodeworks 的资源预览，或在 Blender / three.js 中打开。
