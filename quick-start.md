# 苍穹外卖系统 - 快速开始

## 项目简介
基于Spring Boot的外卖管理系统，包含员工管理、菜品管理、订单处理等核心功能。

## 技术栈
- Spring Boot 2.7.3
- MyBatis + MySQL
- JWT认证
- Lombok + FastJSON

## 核心功能

### 员工登录
- **接口**: POST `/admin/employee/login`
- **安全**: MD5密码加密 + JWT令牌认证
- **异常处理**: 账号不存在、密码错误、账号锁定

### 模块结构
```
sky-take-out/
├── sky-common/     # 公共工具类、常量、异常处理
├── sky-pojo/       # DTO、Entity、VO数据对象
├── sky-server/     # 主业务逻辑、控制器、服务层
```

## 快速部署

### 环境要求
- JDK 8+
- MySQL 5.7+
- Maven 3.6+

### 启动步骤
1. 创建数据库 `sky_take_out`
2. 修改配置文件数据库连接信息
3. 运行 `SkyApplication.main()`

### 访问地址
- 应用: http://localhost:8080
- API文档: http://localhost:8080/doc.html

## 主要特性
- 前后端分离架构
- 统一异常处理
- JWT无状态认证
- 模块化设计
- 自动生成API文档

---
*简单易用的外卖管理系统*