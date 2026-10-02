# COREVERSE 灵核档案

一个可直接运行的单页人格异能测试。当前版本为 **V1.4**，包含 32 道情境题、16 种人格异能、故事化结果档案、专属塔罗式角色牌与六维超能力雷达图。

线上版本：[coreverse-archive.irene1227.chatgpt.site](https://coreverse-archive.irene1227.chatgpt.site)

## 项目结构

```text
.
├── .openai/
│   └── hosting.json   # ChatGPT Sites 静态站点配置
├── dist/
│   ├── index.html     # 完整应用：HTML、CSS、JavaScript 与测试数据
│   └── favicon.svg
├── .gitignore
└── README.md
```

## 本地运行

项目没有构建步骤、第三方依赖、API Key 或后端服务。克隆仓库后，在项目根目录运行：

```bash
python3 -m http.server 8000 --directory dist
```

然后访问 <http://localhost:8000>。

也可以直接用浏览器打开 `dist/index.html`；使用本地 HTTP 服务时，分享与剪贴板等浏览器能力的兼容性更好。

## 部署

这是标准静态网站，将托管平台的发布目录设置为 `dist` 即可，不需要构建命令。

`.openai/hosting.json` 保留了当前 ChatGPT Sites 项目的配置，用于复现现有 Site。若要创建一个全新的 Sites 项目，请先移除其中的 `project_id`，再按新项目流程发布。

## 版本快照

- 版本：V1.4
- 快照日期：2026-10-02
- 页面代码为单文件实现，题目、计分逻辑、16 种结果文案和视觉样式均位于 `dist/index.html`

