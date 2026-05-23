# VECTOUI CONVERTER


 **VectoUI Converter** 支持**一键将蓝湖设计稿转换为 Unity UI Prefab**，并自动搞定资源下载与层级还原，彻底解决手动拼 UI 耗时易错的痛点。如果你想告别枯燥的界面搭建、让 UI 生产效率翻倍，立即访问 [VectoUI 官网 (www.vectoui.com)](https://www.vectoui.com) 开启自动化工作流！



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
----

## 国内 Prepo 镜像

国内 Gitee 仓库镜像 

https://gitee.com/sourcetoken/com.vectoui.unity.convertor

国内资源配置
**manifest.json**
```json

{
  "dependencies": {
    "com.vectoui.unity.convertor": "git@gitee.com:sourcetoken/com.vectoui.unity.convertor.git",
    ...
  }
}    
```