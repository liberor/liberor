<h1 align="center">你好，我是吴小龙 👋</h1>

<p align="center">
  <b>前端开发 / Frontend Developer</b> · Vue3 · React
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

- 具备 **Vue3** 与 **React** 两个完整项目经验，能独立完成从路由鉴权、请求封装到数据可视化的全流程开发。
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
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat-square&logo=pinia&logoColor=black)
![Element Plus](https://img.shields.io/badge/Element%20Plus-409EFF?style=flat-square&logo=element&logoColor=white)
![Ant Design](https://img.shields.io/badge/Ant%20Design-0170FE?style=flat-square&logo=antdesign&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![ECharts](https://img.shields.io/badge/ECharts-AA344D?style=flat-square&logo=apacheecharts&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

## 📌 项目经历

### 🤖 AI 心理健康咨询平台 · `2026.09 – 2026.10`

[在线体验](https://aihealth.liberorreactproject.beer) · [源码](https://github.com/liberor/ai-mental-health)

基于 **React + Vite** 的 AI 心理健康平台，用户 / 管理双端一体。用户端提供 AI 心理咨询、情绪日记、心理知识库与文章阅读；管理端提供数据看板、知识文章管理、咨询记录查看与情绪日志管理。

`React19` `Vite` `TypeScript` `React Router` `Axios` `Ant Design` `Tailwind` `ECharts`

- 完成全部页面开发，搭建用户端与管理端两套路由体系与页面
- 封装 Axios 请求层与响应层：请求拦截注入 token，响应拦截按业务码拆包
- 使用 `IntersectionObserver` 实现知识库文章列表的图片懒加载
- 路由懒加载将首页 JS 从 1.2MB 降至 288KB（**↓76%**），首屏加载从约 5s 优化至约 2s
- **亮点 · SSE 流式对话**：使用 `fetch-event-source` 实现 AI 会话流式输出，通过 `AbortController` 控制中断

### 🛒 商城后台管理系统 · `2026.07 – 2026.10`

[在线体验](https://shopadmin.liberorvueproject.beer) · [源码](https://github.com/liberor/shop-admin)

基于 **Vue3 + Vite** 的 B 端商城后台管理系统，覆盖数据看板、商品多规格 SKU 管理、订单评论、图库管理等 10 余个业务模块。

`Vue3` `Vite` `Vue Router` `Pinia` `Element Plus` `Axios` `WindiCSS` `ECharts`

- 使用 ECharts 绘制统计图表，配合骨架屏、nprogress 加载条、gsap 数字滚动优化体验
- 封装 `FormDrawer` / `TagInput` / `IconSelect` 等通用组件，多页面复用
- 路由懒加载 + Element Plus 按需引入，首屏 JS 从 1.4MB 降至 240KB（**↓83%**），加载从约 6s 优化至约 2s
- **亮点 · RBAC 权限体系**：前端根据后端权限列表动态生成菜单、动态挂载路由，配合自定义指令实现基于角色的权限控制
- **亮点 · SKU 多规格联动**：使用笛卡尔积算法组合多个规格项生成 SKU 表，实现规格增删改排与表格数据实时联动

### 🧩 my-vue3-source · 手写 Vue3 响应式源码

[源码](https://github.com/liberor/my-vue3-source)

从零实现 Vue3 响应式系统核心：`reactive`、`effect`、`ref`、`computed`、`watch`。基于 `Proxy` + `Reflect` 完成依赖收集与派发更新，深入理解 `track` / `trigger`、`Dep`、`scheduler` 。

`TypeScript` `Proxy` `Vue3 源码`

## 
