# Campus Help Platform

一个基于 SpringBoot + Vue 的校园互助平台，帮助学生发布和解决各类问题。

## 项目简介

Campus Help Platform 是一个校园互助服务平台，用户可以：
- 发布求助信息（学业、生活、技能等）
- 回答他人的问题获得积分和声誉
- 个人资料与积分管理
- 实时消息通知
- 问题分类与搜索

## 技术栈

### 后端
- **框架**: Spring Boot 3.x
- **数据库**: MySQL 8.0
- **缓存**: Redis
- **API**: RESTful API
- **认证**: JWT

### 前端
- **框架**: Vue 3
- **UI组件**: Element Plus
- **构建工具**: Vite
- **HTTP客户端**: Axios
- **状态管理**: Pinia

## 项目结构

```
campus-help-platform/
├── backend/                  # 后端项目
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/campushelp/
│   │   │   │   ├── controller/     # 控制器
│   │   │   │   ├── service/        # 业务逻辑
│   │   │   │   ├── mapper/         # 数据映射
│   │   │   │   ├── entity/         # 实体类
│   │   │   │   ├── dto/            # 数据传输对象
│   │   │   │   ├── config/         # 配置类
│   │   │   │   ├── utils/          # 工具类
│   │   │   │   └── CampusHelpApplication.java
│   │   │   └── resources/
│   │   │       ├── application.yml  # 配置文件
│   │   │       └── db/
│   │   │           └── init.sql    # 数据库初始化
│   │   └── test/
│   ├── pom.xml
│   └── README.md
├── frontend/                 # 前端项目
│   ├── src/
│   │   ├── components/      # 通用组件
│   │   ├── views/           # 页面组件
│   │   ├── router/          # 路由配置
│   │   ├── stores/          # 状态管理
│   │   ├── utils/           # 工具函数
│   │   ├── api/             # API请求
│   │   ├── App.vue
│   │   └── main.js
│   ├── public/
│   ├── package.json
│   ├── vite.config.js
│   └── README.md
└── docs/                     # 文档
    ├── API.md
    ├── DATABASE.md
    └── DEPLOYMENT.md
```

## 快速开始

### 前置要求
- JDK 17+
- Node.js 18+
- MySQL 8.0+
- Redis 6.0+

### 后端启动

```bash
cd backend
mvn clean install
mvn spring-boot:run
```

### 前端启动

```bash
cd frontend
npm install
npm run dev
```

## API 文档

详见 [API文档](docs/API.md)

## 数据库设计

详见 [数据库设计](docs/DATABASE.md)

## 部署指南

详见 [部署指南](docs/DEPLOYMENT.md)

## License

MIT
