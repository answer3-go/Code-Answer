# Code Answer

**版本：v2.3.0 (2025-06-13)**

一个现代化的编程学习助手，集成AI资讯、LeetCode每日题目和GitHub热门项目，为程序员提供全方位的学习支持。

## 更新日志

### v2.3.0 (2025-06-13)
#### 🔧 用户注册系统重构版本

**重要更新：**
- ✅ **注册流程简化**：移除"谁是Answer"验证问题，简化用户注册流程
- ✅ **独立密码系统**：新注册用户可设置个人密码，不再依赖固定密码
- ✅ **密码安全增强**：添加密码长度验证和确认密码功能
- ✅ **用户数据管理**：优化用户数据存储结构，支持用户名和密码独立管理

**功能改进：**
- 🔐 **注册界面优化**：新增密码输入和确认密码输入框
- 🔐 **登录验证升级**：支持默认用户固定密码和注册用户独立密码双重验证模式
- 🔐 **数据安全存储**：用户密码安全存储在本地配置文件中
- 🔐 **用户体验提升**：改进错误提示信息和键盘导航体验

### v2.2.0 (2025-06-02)
#### 📚 文档更新与功能优化版本

**重要更新：**
- ✅ **文档全面更新**：更新README文档，移除已废除功能描述，与实际实现保持一致
- ✅ **功能描述修正**：准确描述三列布局设计和实际功能特性
- ✅ **用户体验优化**：完善登录验证系统和启动流程说明

**文档改进：**
- 📝 **功能特点更新**：移除"编程知识学习"等已废除功能，突出LeetCode和GitHub功能
- 📝 **界面布局说明**：明确描述三列布局：AI新闻、LeetCode题目、GitHub项目
- 📝 **技术特色新增**：添加前端设计和数据处理的技术特色说明
- 📝 **使用指南完善**：提供详细的交互操作指南

**技术架构说明：**
- 🔧 **CustomTkinter框架**：现代化GUI界面设计
- 🔧 **模块化架构**：独立的爬虫模块和数据服务
- 🔧 **智能缓存系统**：本地JSON缓存，提高响应速度
- 🔧 **异步数据加载**：后台线程处理，不阻塞界面

## 功能特点

- **AI新闻浏览**：自动获取AI领域最新动态，支持点击阅读原文和预览功能
- **LeetCode每日题目**：提供每日算法题目，支持难度分级和详细查看
- **GitHub热门项目**：展示每日GitHub热门项目，包含项目信息和直接访问链接
- **深色/浅色主题**：支持切换深色和浅色界面模式
- **用户登录验证**：支持用户注册和登录验证系统
- **启动动画**：精美的启动欢迎界面，包含复杂动画效果
- **定期更新**：支持一键刷新最新内容，智能缓存机制

## 界面布局

应用采用现代化三列布局设计：
- **左列**：AI领域最新动态
- **中列**：LeetCode每日题目
- **右列**：GitHub热门项目

## 安装使用

### 方法1：直接运行可执行文件（推荐）

1. 下载发布的可执行文件：`Code Answer.exe`
2. 双击运行程序，无需安装Python环境

### 方法2：从源码运行

1. 确保已安装Python 3.8或更高版本
2. 克隆或下载本仓库
3. 安装依赖库：
   ```
   pip install -r requirements.txt
   ```
4. 运行程序：
   ```
   python main.py
   ```

## 数据来源

- **AI新闻**：来自各大科技媒体的RSS源和专业AI资讯网站
- **LeetCode题目**：通过LeetCode官方API获取真实题目数据
- **GitHub项目**：爬取GitHub Trending页面获取热门项目信息

## 启动流程

应用启动时会依次显示：

1. **启动欢迎界面**：包含logo动画、标题滑入、粒子效果等复杂动画
2. **用户登录验证**：支持用户名密码验证和新用户注册
3. **主应用界面**：三列布局展示各类内容

## 核心功能详解

### AI新闻获取

- **多源获取**：从AI Trend、AI话题、Synced等网站爬取最新AI新闻
- **智能解析**：自动解析网页内容，提取标题、来源、发布时间、摘要和链接
- **时间排序**：按发布时间排序，确保展示最新内容
- **预览功能**：支持新闻预览窗口，无需跳转即可查看详情
- **缓存机制**：支持本地缓存，减少重复请求，提高加载速度

### LeetCode题目系统

- **真实题目**：通过LeetCode API获取真实的算法题目
- **难度分级**：支持Easy、Medium、Hard三个难度等级
- **智能选择**：每日自动选择不同难度的题目组合
- **历史记录**：记录已查看题目，避免重复显示
- **详细查看**：支持题目详情窗口，包含完整题目描述和解题思路
- **重置功能**：支持重置题目历史记录

### GitHub热门项目

- **实时热门**：获取GitHub每日、每周、每月热门项目
- **项目信息**：显示项目名称、描述、编程语言、星标数等
- **直接访问**：点击项目标题直接跳转到GitHub页面
- **README预览**：自动获取项目README内容进行预览

## 技术特色

### 前端设计
- **CustomTkinter**：使用现代化的GUI框架，提供美观的界面
- **响应式布局**：支持窗口缩放和自适应布局
- **动画效果**：丰富的启动动画和交互效果
- **主题系统**：完整的深浅主题切换支持

### 数据处理
- **智能爬虫**：多网站数据爬取，错误处理和重试机制
- **缓存系统**：本地JSON缓存，提高响应速度
- **数据去重**：防止重复内容显示
- **异步加载**：后台线程加载数据，不阻塞界面

## 环境要求

- Python 3.8+
- customtkinter 5.2.2 (现代化GUI界面)
- requests 2.32.3 (网络请求)
- beautifulsoup4 4.13.4 (HTML解析)
- pillow 11.2.1 (图像处理)
- feedparser 6.0.11 (RSS解析)

## 目录结构

```
project_root/
├── main.py                # 启动入口
├── gui/                   # 所有UI界面逻辑
│   ├── app.py             # 主应用界面
│   ├── login_dialog.py    # 登录验证界面
│   ├── splash_screen.py   # 启动欢迎界面
│   ├── github_frame.py    # GitHub项目展示框架
│   ├── algorithm_view.py  # 算法题查看窗口
│   └── settings_dialog.py # 设置对话框
├── services/              # 服务逻辑
│   ├── data_service.py    # 数据服务整合
│   ├── news_scraper.py    # 新闻爬虫服务
│   ├── leetcode_scraper.py # LeetCode爬虫服务
│   └── github_scraper.py  # GitHub爬虫服务
├── cache/                 # 缓存目录
├── assets/                # 资源文件
│   ├── logo.ico           # 应用图标
│   └── logo.png           # 应用Logo
└── requirements.txt       # 项目依赖
```

## 使用说明

1. **启动应用**：运行程序后会显示启动动画和登录界面
2. **用户验证**：输入用户名和密码进行验证，支持新用户注册
3. **浏览内容**：在三列布局中浏览AI新闻、LeetCode题目和GitHub项目
4. **交互功能**：
   - 点击新闻标题查看预览或跳转原文
   - 点击"查看详情"按钮查看LeetCode题目完整内容
   - 点击GitHub项目标题直接访问项目页面
5. **刷新内容**：使用各区域的"刷新"按钮获取最新内容
6. **主题切换**：使用右上角按钮切换深色/浅色主题

## 常见问题

- **无法获取数据**：检查网络连接，或点击"刷新"按钮重试
- **界面显示异常**：尝试切换深色/浅色模式
- **程序闪退**：检查是否缺少依赖库，或查看错误日志
- **登录失败**：确认用户名密码正确，或注册新用户

## 隐私说明

本程序仅通过互联网获取公开信息，不会收集任何用户个人数据。用户登录信息仅存储在本地配置文件中。

## 开源协议

本项目采用MIT协议开源，欢迎贡献和改进！

## 网络要求

- 本应用需要网络连接以获取最新AI新闻、LeetCode题目和GitHub项目
- 如果网络连接不可用，应用将使用本地缓存的内容
- 首次运行建议保持网络连接以获取初始数据

## 未来计划

- 收藏和标记已读功能
- 用户自定义内容源添加
- 学习进度跟踪和统计
- 搜索和过滤功能
- 更多编程语言和技术栈支持
- 移动端适配 