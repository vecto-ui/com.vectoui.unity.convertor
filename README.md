# VECTOUI UNITY CONVERTER

## 相关文档

- [官网 vectoui.com](https://www.vectoui.com/)

- [接入文档](https://www.vectoui.com/docs/getting-started/integration-guide)

## 插件介绍

此项目为 VectoUI 针对 Unity3D 引擎开发的 UI 转换工具

## 接入方式

在 Unity 项目中，通过在 `Packages/manifest.json` 中添加以下配置, 以引入本插件 (默认用户已配置 [SSH-Key](https://docs.github.com/zh/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) 的鉴权方式)

**manifest.json**
```json

{
  "dependencies": {
    "com.vectoui.unity.convertor": "git@github.com:vecto-ui/com.vectoui.unity.convertor.git",
    ...
  }
}    
```
