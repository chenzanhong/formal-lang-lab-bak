# FormalLangLab
（项目介绍，非实际仓库）

FormalLangLab 是一个基于 Web 的交互式形式语言与自动机学习系统，旨在帮助计算机科学专业的学生更直观、高效地理解文法、正则表达式、自动机（DFA/NFA）等形式语言与自动机核心概念。该项目集成了自动机可视化、文法合法性检查、DFA/NFA 构造与转换、字符串接受判断的分析过程演示等功能，并集成 AI 模块提供智能辅助学习功能。

## 功能模块

- **文法处理**：文法合法性验证、文法类型判断、文法简化（去无用符号、单一产生式等）、字符串识别与分析
- **自动机操作**：DFA/NFA 构造与验证、NFA 转 DFA 算法实现、DFA 最小化、自动机字符串接受判断，前端支持可视化自动机编辑
- **正则表达式**：正则表达式验证、字符串匹配
- **转换功能**：文法与自动机之间的相互转换、正则表达式与自动机之间的相互转换
- **学习资料**：形式语言与自动机理论知识库、学习资料管理
- **AI 辅助功能**：页面感知，AI问答
- **用户管理**：用户注册、登录认证、JWT token 管理、邮件验证功能

## 技术栈

### 后端

- **框架**: Golang (Gin)
- **数据库**: PostgreSQL
- **ORM**: GORM
- **缓存**: Redis
- **认证**: JWT
- **文件存储**: 阿里云OSS SDK
- **消息队列**: Kafka（用于邮件异步处理）
- **AI集成**: 支持本地 Ollama 或远程 API（通义千问）
- **向量数据库**: Chroma（待确定）
- **日志**: Zap 结构化日志系统
- **配置管理**: YAML 配置文件
- **中间件**: CORS
- **工具库**: HTTP Client、Cryptoutil、Token
- **监控**: Prometheus + Grafana

### 前端
- **核心框架**: React 19, TypeScript
- **构建工具**: Vite
- **UI组件库**: Material-UI (MUI), TailwindCSS, HeadlessUI, Heroicons
- **可视化**: D3.js, React Flow, Dagre
- **动画**: Framer Motion
- **路由**: React Router DOM
- **状态管理/数据获取**: React Query
- **数学公式**: KaTeX, react-katex
- **代码编辑/高亮**: React Simple Code Editor, PrismJS, Highlight.js
- **文档处理**: Marked, React Markdown, Remark/Gfm
- **网络请求**: Axios
- **认证**: JWT Decode
- **样式解决方案**: Emotion
- **开发工具**: ESLint, Prettier, PostCSS
