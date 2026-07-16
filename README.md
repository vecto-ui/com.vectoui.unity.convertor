# VectoUI Unity Converter

## 简介

VectoUI Unity Converter 是 VectoUI 面向 Unity 的 UI 自动化生成插件。它支持从 VectoUI、Figma 以及 Lanhu 读取设计稿数据，并在 Unity 中自动生成可编辑的 UI Prefab。

通过 VDS，VectoUI 可以将不同设计来源的数据统一为可生成、可管理、可复用的 UI 数据。Unity 团队可以在插件中选择目标数据源和设计稿，自动完成 UI 层级、节点位置、图片引用、文本配置等内容的生成，减少手动拼 UI 和重复还原工作。

访问 [VectoUI 官网](https://www.vectoui.com/) 了解产品能力、工作流、下载入口、价格方案与最新文档。

## 核心能力

- **多数据源接入**：支持 VectoUI、Figma 以及 Lanhu 三类设计稿数据来源。
- **UI Prefab 自动生成**：在 Unity 中选择设计稿后自动生成可编辑的 UI Prefab。
- **减少手动拼 UI**：减少手动还原层级、位置、图片引用和文本配置的重复工作。
- **VDS 数据统一**：通过 VDS 标准化描述 UI 层级、坐标尺寸、图片资源、字体和样式数据。
- **适配团队工程流程**：生成结果可继续在 Unity 中编辑，并可结合项目规范进行组件绑定、字体映射和后处理扩展。

## 支持的数据源

| 数据源 | 说明 | 典型链路 |
| --- | --- | --- |
| VectoUI | 读取通过 VectoUI Photoshop / Sketch 插件上传到 VectoUI 空间的设计稿数据 | Photoshop / Sketch -> VectoUI 空间 -> VectoUI Unity Converter -> UI Prefab |
| Figma | 读取 Figma 团队、项目和设计文件 | Figma 设计稿 -> VectoUI Unity Converter -> UI Prefab |
| Lanhu | 读取 Lanhu 中的设计稿数据 | Lanhu 设计稿 -> VectoUI Unity Converter -> UI Prefab |

## 相关地址

| 名称 | 地址 |
| --- | --- |
| VectoUI 官网 | https://www.vectoui.com/ |
| Unity 插件下载页 | https://www.vectoui.com/downloads/unity-plugin |
| Photoshop 插件下载页 | https://www.vectoui.com/downloads/photoshop-plugin |
| Sketch 插件下载页 | https://www.vectoui.com/downloads/sketch-plugin |
| Lanhu 到 Unity 工作流 | https://www.vectoui.com/features/lanhu-to-unity |
| Figma 到 Unity 工作流 | https://www.vectoui.com/features/figma-to-unity |
| GitHub 仓库 | https://github.com/vecto-ui/com.vectoui.unity.convertor |
| Gitee 镜像 | https://gitee.com/sourcetoken/com.vectoui.unity.convertor |

## 安装方式

### 通过 Unity Package Manager 安装

在 Unity 项目的 `Packages/manifest.json` 中添加以下配置，即可通过 Unity Package Manager 引入 VectoUI Unity Converter。使用 SSH 地址时，需要先完成对应 Git 平台的 SSH Key 配置。

GitHub:

```json
{
  "dependencies": {
    "com.vectoui.unity.convertor": "git@github.com:vecto-ui/com.vectoui.unity.convertor.git"
  }
}
```

Gitee:

```json
{
  "dependencies": {
    "com.vectoui.unity.convertor": "git@gitee.com:sourcetoken/com.vectoui.unity.convertor.git"
  }
}
```

也可以在 Unity Editor 中打开 `Window > Package Manager`，点击左上角 `+`，选择 `Install package from git URL...`，然后输入 GitHub 或 Gitee 的插件仓库地址。

## 基础使用流程

1. 在 Unity 项目中安装 VectoUI Unity Converter。
2. 打开 VectoUI Unity Converter 插件窗口。
3. 配置 VectoUI API Key。
4. 选择数据源：VectoUI、Figma 或 Lanhu。
5. 选择目标项目和设计稿。
6. 点击生成，自动生成可编辑的 UI Prefab。
7. 根据项目需要继续进行组件绑定、字体映射和后处理扩展。

## 文档与工作流

| 内容 | 地址 |
| --- | --- |
| Unity 插件接入文档 | https://www.vectoui.com/docs/getting-started/integration-guide |
| Unity 插件高级使用 | https://www.vectoui.com/docs/getting-started/vu-advanced-usage |
| Figma 配置文档 | https://www.vectoui.com/docs/getting-started/figma-support |
| Photoshop 插件下载 | https://www.vectoui.com/downloads/photoshop-plugin |
| Sketch 插件下载 | https://www.vectoui.com/downloads/sketch-plugin |
| Lanhu 到 Unity 工作流 | https://www.vectoui.com/features/lanhu-to-unity |
| Figma 到 Unity 工作流 | https://www.vectoui.com/features/figma-to-unity |

---

# VectoUI Unity Converter

## Overview

VectoUI Unity Converter is the Unity-side UI automation plugin for VectoUI. It supports design data from VectoUI, Figma, and Lanhu, and generates editable UI Prefabs inside Unity.

With VDS, VectoUI turns different design sources into generateable, manageable, and reusable UI data. Unity teams can select a data source and a design file in the plugin, then generate UI hierarchy, node positions, image references, text configuration, and related UI content automatically, reducing manual UI assembly and repetitive rebuilding work.

Visit the [VectoUI website](https://www.vectoui.com/en) to learn about product capabilities, workflows, downloads, pricing, and the latest documentation.

## Core Capabilities

- **Multiple data sources**: Supports design data from VectoUI, Figma, and Lanhu.
- **UI Prefab generation**: Select a design file in Unity and generate an editable UI Prefab automatically.
- **Less manual UI assembly**: Reduces repetitive work around rebuilding hierarchy, positions, image references, and text configuration by hand.
- **Unified VDS data**: Uses VDS to standardize UI hierarchy, coordinates, dimensions, image assets, fonts, and style data.
- **Fits team engineering workflows**: Generated results remain editable in Unity and can be extended with component binding, font mapping, and post-processing logic based on project conventions.

## Supported Data Sources

| Data Source | Description | Typical Workflow |
| --- | --- | --- |
| VectoUI | Reads design data uploaded to VectoUI Space through the VectoUI Photoshop / Sketch plugins | Photoshop / Sketch -> VectoUI Space -> VectoUI Unity Converter -> UI Prefab |
| Figma | Reads Figma teams, projects, and design files | Figma design -> VectoUI Unity Converter -> UI Prefab |
| Lanhu | Reads design data from Lanhu | Lanhu design -> VectoUI Unity Converter -> UI Prefab |

## Links

| Name | URL |
| --- | --- |
| VectoUI Website | https://www.vectoui.com/en |
| Unity Plugin Download | https://www.vectoui.com/en/downloads/unity-plugin |
| Photoshop Plugin Download | https://www.vectoui.com/en/downloads/photoshop-plugin |
| Sketch Plugin Download | https://www.vectoui.com/en/downloads/sketch-plugin |
| Lanhu to Unity Workflow | https://www.vectoui.com/en/features/lanhu-to-unity |
| Figma to Unity Workflow | https://www.vectoui.com/en/features/figma-to-unity |
| GitHub Repository | https://github.com/vecto-ui/com.vectoui.unity.convertor |
| Gitee Mirror | https://gitee.com/sourcetoken/com.vectoui.unity.convertor |

## Installation

### Install with Unity Package Manager

Add the following dependency to `Packages/manifest.json` in your Unity project to install VectoUI Unity Converter through Unity Package Manager. SSH URLs require SSH Key access on the selected Git platform.

GitHub:

```json
{
  "dependencies": {
    "com.vectoui.unity.convertor": "git@github.com:vecto-ui/com.vectoui.unity.convertor.git"
  }
}
```

Gitee:

```json
{
  "dependencies": {
    "com.vectoui.unity.convertor": "git@gitee.com:sourcetoken/com.vectoui.unity.convertor.git"
  }
}
```

You can also open `Window > Package Manager` in the Unity Editor, click `+`, choose `Install package from git URL...`, and enter the GitHub or Gitee repository URL for the plugin.

## Basic Usage

1. Install VectoUI Unity Converter in your Unity project.
2. Open the VectoUI Unity Converter plugin window.
3. Configure your VectoUI API Key.
4. Select a data source: VectoUI, Figma, or Lanhu.
5. Select the target project and design file.
6. Generate an editable UI Prefab automatically.
7. Continue with component binding, font mapping, and post-processing extensions as needed for your project.

## Documentation and Workflows

| Content | URL |
| --- | --- |
| Unity Plugin Integration Guide | https://www.vectoui.com/en/docs/getting-started-en/integration-guide-en |
| Unity Plugin Advanced Usage | https://www.vectoui.com/en/docs/getting-started-en/vu-advanced-usage-en |
| Figma Configuration Guide | https://www.vectoui.com/en/docs/getting-started-en/figma-support-en |
| Photoshop Plugin Download | https://www.vectoui.com/en/downloads/photoshop-plugin |
| Sketch Plugin Download | https://www.vectoui.com/en/downloads/sketch-plugin |
| Lanhu to Unity Workflow | https://www.vectoui.com/en/features/lanhu-to-unity |
| Figma to Unity Workflow | https://www.vectoui.com/en/features/figma-to-unity |
