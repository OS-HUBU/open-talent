# OpenTalent: 开源人才评价与服务平台

## 项目简介

**OpenTalent** 是一个基于 Git 行为数据的开源人才评价与服务平台，旨在通过数据驱动的方式，客观、公正地评价开发者的开源贡献。我们希望通过透明、开放的评价体系，为开发者提供反馈，并帮助雇主发现和培养优质的开源人才。

## 功能特性

- **贡献分析**：基于 Git 数据，量化开发者在代码、文档、测试、治理、运营等方面的贡献。
- **开源影响力评分**：通过贡献的广度与深度，基于 OpenRank 算法评估开发者在开源项目中的影响力。
- **社区互动度**：分析开发者在开源社区中的活跃度，包括 issue、PR、讨论等互动行为。
- **定制化报告**：为开发者和企业提供详细的贡献与影响力报告，便于展示技能和发展职业生涯。
- **开源职业发展建议**：根据开发者的表现，提供个性化的职业发展建议和机会。

## 项目结构

```plaintext
├── backend                # 后端服务目录
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/           # Java 源码目录
│   │   │   │   └── com/
│   │   │   │       └── example/
│   │   │   │           └── opentalent/   # 主业务包，包含控制器、服务、实体、仓库等
│   │   │   └── resources/      # Spring Boot 配置文件和资源文件目录
│   │   │       ├──  db
│   │   │       ├──  mapper
│   │   │       └──  application.yml   # 应用配置文件
│   │   │       ├──  template.xlsx
│   │   └── test/               # 单元测试目录
│   └── .mvn/wrapper                 # Maven Wrapper配置
│   └── .gitattributes               # Git 属性配置
│   └── .gitignore                   # 
│   └──  mvnw                        #
│   └──  mvnw.cmd                    # Maven Wrapper脚本
│   └── pom.xml                      # Maven 构建配置文件
├── frontend               # 前端项目目录
│   ├── public/              # 公共静态资源目录
│   ├── src/                 # Vue源码目录
│   └── .gitignore   
│   └── .browserslistrc	     
│   └── babel.config.js	     # Babel转码配置
│   └── jsconfig.json
│   └── package.json         # 前端依赖和脚本定义
│   └── package-lock.json   
│   └── vue.config.js
```

## 安装与使用

### 1. 克隆项目

```bash
git clone https://github.com/x-lab/OpenTalent.git
cd OpenTalent
```

### 2. 创建数据库并初始化
执行 src/main/resources/db/init.sql 中的 SQL 脚本来初始化表结构和数据

###  3. 配置数据库连接
编辑 src/main/resources/application.yml，根据你的本地环境配置数据库信息：
```bash
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/open_talent?serverTimezone=UTC
    username: your_username
    password: your_password
```

### 4. 使用 Maven 构建项目

### 5. 启动后端服务


## 贡献指南

我们欢迎任何形式的贡献！您可以通过以下方式参与：

1. 提交 Issue 来报告错误或建议新功能。
2. 提交 Pull Request 来修复问题或添加新功能。
3. 提交文档改进或翻译。

### 开发流程

1. Fork 该仓库。
2. 创建您的功能分支：`git checkout -b feature/your-feature-name`。
3. 提交您的更改：`git commit -m 'Add some feature'`。
4. Push 到远程仓库：`git push origin feature/your-feature-name`。
5. 创建一个 Pull Request。

## 许可证

本项目基于 [木兰宽松](LICENSE) 开源许可。

## 联系我们

如果您有任何问题或建议，请通过以下方式联系我们：

- 项目主页：[https://github.com/X-lab2017/open-talent/](https://github.com/X-lab2017/open-talent/)
- 邮件：[contact@opentalent.io](mailto:contact@opentalent.io)

## 致谢

感谢所有为开源社区做出贡献的开发者！
