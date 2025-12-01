# FormalLangLab Frontend

**支持自动机可视化的形式语言学习系统 - 前端模块**

## 🎯 项目概述

FormalLangLab是一个集形式语言理论学习、自动机可视化编辑与模拟、文法分析与转换为一体的综合学习平台。前端模块基于现代Web技术栈构建，提供直观的用户界面和丰富的交互功能，帮助用户更好地理解和学习形式语言与自动机理论。

### 核心功能

- **自动机可视化编辑与模拟**：支持有限自动机（DFA/NFA）的交互式创建、编辑和模拟运行
- **文法分析与转换**：提供上下文无关文法（CFG）的编辑、分析和转换功能
- **正则表达式处理**：支持正则表达式的验证、测试和转换为自动机
- **学习资源中心**：提供形式语言与自动机理论的学习资料和知识库
- **资源存储管理**：用户可保存和管理创建的自动机、文法和正则表达式
- **AI智能助手**：提供学习指导和问题解答

## 🛠️ 技术栈

- **框架**：React 18
- **语言**：TypeScript
- **构建工具**：Vite
- **样式方案**：Tailwind CSS + MUI (Material-UI)
- **状态管理**：React Context API
- **路由**：React Router
- **HTTP客户端**：Axios
- **代码规范**：ESLint + Prettier

## 📁 目录结构

```
frontend/
├── public/           # 静态资源
│   ├── content/      # 内容文件
│   └── vite.svg      # 项目图标
├── src/              # 源代码
│   ├── api/          # API请求相关
│   ├── assets/       # 静态资源
│   ├── components/   # 可复用组件
│   ├── contexts/     # 上下文管理
│   ├── data/         # 模拟数据
│   ├── pages/        # 页面组件
│   ├── styles/       # 全局样式
│   ├── types/        # TypeScript类型定义
│   ├── utils/        # 工具函数
│   ├── App.tsx       # 应用入口组件
│   └── main.tsx      # 应用入口文件
├── docs/             # 开发文档
├── .eslintrc.cjs     # ESLint配置
├── .prettierrc       # Prettier配置
├── package.json      # 项目依赖配置
├── tailwind.config.js # Tailwind CSS配置
├── tsconfig.json     # TypeScript配置
└── vite.config.ts    # Vite配置
```

## 📦 功能模块详情

### 1. 自动机编辑器

提供直观的拖拽式界面，支持自动机节点和边的创建、编辑、删除。实现自动机的可视化展示和字符串识别模拟。

位置：`src/pages/Automaton/`

### 2. 文法编辑器

支持上下文无关文法的定义、编辑和分析。提供文法推导、有效性验证等功能。

位置：`src/pages/Grammar/`

### 3. 正则表达式工具

提供正则表达式的输入、测试和验证功能。支持将正则表达式转换为NFA和DFA。

位置：`src/pages/Regex/`

### 4. 学习资源中心

提供形式语言与自动机理论的学习资料、教程和知识点详情。

位置：`src/pages/Learn/`

### 5. 资源存储

允许用户保存和管理创建的自动机、文法和正则表达式。支持分页展示和搜索。

位置：`src/pages/Store/`

### 6. 用户认证

提供用户注册、登录和密码找回功能。

位置：`src/pages/Auth/`