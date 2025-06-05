# 待办事项列表Web应用

一个基于Vue.js + Spring Boot的全栈Web应用，实现员工管理和待办事项功能。

## 项目结构

```
todolist-web-app/
├── frontend/          # Vue.js前端项目
│   ├── src/
│   │   ├── components/  # 组件
│   │   ├── views/      # 页面
│   │   ├── router/     # 路由配置
│   │   └── assets/     # 静态资源
│   ├── public/        # 公共文件
│   ├── package.json   # 前端依赖配置
│   └── ...
├── backend/           # Spring Boot后端项目
│   ├── src/main/java/ # Java源码
│   ├── src/main/resources/ # 配置文件
│   ├── pom.xml        # Maven配置
│   └── ...
└── README.md          # 项目说明
```

## 技术栈

### 前端
- **Vue.js 3** - 渐进式JavaScript框架
- **Element Plus** - Vue 3组件库
- **Vue Router** - 客户端路由
- **Axios** - HTTP请求库

### 后端
- **Spring Boot 3.4.6** - Java企业级开发框架
- **MyBatis Plus 3.5.6** - 持久层框架
- **MySQL** - 关系型数据库
- **Maven** - 项目构建工具

## 功能特性

- ✅ 员工信息管理
- ✅ 分页查询
- ✅ 数据表格展示
- ✅ 响应式界面设计
- ✅ 待办事项管理
- ✅ 任务状态切换

## 快速开始

### 前端启动

```bash
cd frontend
npm install
npm run serve
```

前端将在 http://localhost:8080 启动

### 后端启动

1. 确保已安装Java 17和MySQL数据库
2. 创建数据库`neuedu`
3. 修改`backend/src/main/resources/application.properties`中的数据库连接信息
4. 启动后端服务：

```bash
cd backend
./mvnw spring-boot:run
```

后端将在 http://localhost:8080/springbootmybatisplus04 启动

## 开发说明

### 数据库配置

后端默认连接配置：
- 数据库：MySQL
- 端口：3306
- 数据库名：neuedu
- 用户名：root
- 密码：12345678

请根据实际情况修改`backend/src/main/resources/application.properties`文件。

### API接口

- 基础路径：`http://localhost:8080/springbootmybatisplus04`
- 员工分页查询：`GET /emp/getPage`

## 许可证

MIT License