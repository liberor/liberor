<h1 align="center">你好，我是吴小龙 👋</h1>

<p align="center">
  <b>前端开发 / Frontend Developer</b> · Vue3 · React · Node.js
</p>


<p align="center">
  🎓 武汉理工大学 · 软件工程（卓越工程师）　2024.09 – 至今
</p>
<p align="center">
  <a href="mailto:1483538307@qq.com"><img src="https://img.shields.io/badge/Email-1483538307@qq.com-blue?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://github.com/liberor"><img src="https://img.shields.io/badge/GitHub-liberor-181717?style=flat-square&logo=github" alt="GitHub"></a>
</p>


---

## 🧑‍💻 关于我

- 具备 **Vue3** 与 **React** 两个完整项目经验，并熟悉 **Node.js BFF / SSE / RAG / Function Calling**，能独立完成从前端页面到 AI 应用落地的全流程开发。
- 了解 RAG 全链路与 LLM 流式对接，熟悉 Prompt 工程、MCP 协议与 AI Skill 开发。
- 熟悉 Vite / Webpack 与模块化开发、代码分包、性能优化；了解 HTTP/TCP 协议、浏览器渲染与同源策略。
- 熟悉部分 **Vue3 源码**，能手写 `reactive` / `effect` / `ref` / `computed` / `watch` 等核心模块。
- 算法与基础扎实：**LeetCode 200+**，完成 **CSAPP** 的 `data` / `bomb` / `attack` / `cache` 四个 lab。
- 英语 **CET-6 595**，能阅读英文文档与框架源码。
- 对前端技术有热情，乐于追根溯源，学习与迁移能力强。

## 🛠 技术栈

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vue3](https://img.shields.io/badge/Vue3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Webpack](https://img.shields.io/badge/Webpack-8DD6F9?style=flat-square&logo=webpack&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat-square&logo=pinia&logoColor=black)
![Element Plus](https://img.shields.io/badge/Element%20Plus-409EFF?style=flat-square&logo=element&logoColor=white)
![ECharts](https://img.shields.io/badge/ECharts-AA344D?style=flat-square&logo=apacheecharts&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

## 📌 项目经历

### 🤖 AI Agent 对话与多模态生成平台 · `2026.09 – 2026.10`

[在线体验](https://aichat.liberorreactproject.beer) · [源码](https://github.com/liberor/aichat)

基于 **React + Node.js** 的 AI Agent 平台，支持多模型接入（BYOK）、SSE 断流续传、RAG 知识库检索、自定义 Skill / Prompt，可通过 MCP（Streamable HTTP）接入外部工具，并提供文生图 / 文生视频能力。

`React19` `TypeScript` `Vite` `Node.js` `Express`

- **流式输出**：基于浏览器原生 `EventSource` 接收 SSE 事件，结合 `ReactMarkdown` 实时渲染流式内容。
- **断流续传**：流式输出时关闭标签页、刷新页面或网络中断后无需重新提问，自动从断点恢复，避免重复生成与 token 浪费。
- **工具调用**：解析 OpenAI 兼容流式 `tool_calls` 分片（按 `index` 聚合参数），支持 RAG、Skill、MCP 与视频 / 图片生成工具。
- **任务状态反馈**：封装 `ToolCard` 组件实时展示 Function Calling 执行状态，包含工具名、函数参数、累计耗时与进度条；执行完毕后渲染调用结果。
- **RAG 全链路**：文档解析与切片后调用百炼 Embedding 模型完成向量化；查询阶段先通过余弦相似度召回候选切片，再经 Rerank 模型重排，最终将相关性最高的切片注入 LLM 上下文。
- **Prompt 组装**：使用当前日期、Agent 人设、Skill、RAG 上下文拼接成 System Prompt 传给 LLM；Skill 采用渐进式披露，RAG 上下文片段声明为数据而非指令，降低提示词注入风险。

### 🛒 商城后台管理系统 · `2026.07 – 2026.09`

[在线体验](https://shopadmin.liberorvueproject.beer) · [源码](https://github.com/liberor/shop-admin)

基于 **Vue3 + Vite** 的 B 端商城后台管理系统，覆盖数据看板、商品多规格 SKU 管理、订单评论、图库管理等业务模块。

`Vue3` `Vite` `Vue Router` `Pinia` `Element Plus` `Axios` `WindiCSS` `ECharts`

- **交互体验优化**：使用 ECharts 绘制统计图表，配合骨架屏、nprogress 加载条、gsap 数字滚动优化体验
- **通用组件封装**：封装 `FormDrawer` / `TagInput` / `IconSelect` 等通用组件，让多个业务页面复用，提高开发效率
- **前端性能优化**：路由懒加载 + Element Plus / ECharts 按需引入，首屏 JS 从 1.4MB 降至 240KB（**↓83%**）
- **RBAC 权限体系**：前端根据后端权限列表动态生成菜单、动态挂载路由，配合自定义指令实现基于角色的权限控制
- **SKU 多规格联动**：使用回溯算法组合多个规格项生成 SKU 表，实现规格增删改排与表格数据实时联动

### 🧩 my-vue3-source · 手写 Vue3 响应式源码

[源码](https://github.com/liberor/my-vue3-source)

从零实现 Vue3 响应式系统核心：`reactive`、`effect`、`ref`、`computed`、`watch`。基于 `Proxy` + `Reflect` 完成依赖收集与派发更新，深入理解 `track` / `trigger`、`Dep`、`scheduler` 。

`TypeScript` `Proxy` `Vue3 源码`

## 
