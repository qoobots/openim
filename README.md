# 微信 Flutter 客户端

一个使用 Flutter 开发的微信风格即时通讯应用，实现了微信的核心功能和界面。

## 功能特性

### 聊天功能
- 聊天列表（支持搜索、下拉刷新、左滑删除）
- 聊天详情页（文字消息、语音输入、表情发送）
- 消息长按菜单（复制、转发、收藏、编辑、删除）
- 更多功能面板（图片、拍摄、视频、位置、红包、转账、文件、名片）
- 视频/语音通话界面

### 通讯录
- 字母索引侧边栏
- 按拼音首字母分组显示
- 联系人搜索
- 联系人详情页（发消息、语音/视频通话）

### 朋友圈
- 朋友圈动态展示
- 图片九宫格展示
- 图片预览（支持缩放）
- 点赞、评论功能
- 发布动态

### 发现
- 朋友圈入口
- 视频号、直播、搜一搜、附近
- 购物、游戏、小程序入口

### 个人中心
- 个人信息展示与编辑
- 服务、收藏、朋友圈、卡包、表情
- 设置页面

### 其他功能
- 启动页动画
- 红包发送与领取
- 视频/语音通话界面

## 项目结构

```
lib/
├── main.dart                 # 应用入口
├── models/                   # 数据模型
│   ├── chat.dart            # 聊天模型
│   ├── contact.dart         # 联系人模型
│   └── message.dart         # 消息模型
└── pages/                    # 页面
    ├── chat_list_page.dart       # 聊天列表页
    ├── chat_detail_page.dart     # 聊天详情页
    ├── contacts_page.dart        # 通讯录页
    ├── contact_detail_page.dart  # 联系人详情页
    ├── discover_page.dart        # 发现页
    ├── moments_page.dart         # 朋友圈页
    ├── profile_page.dart         # 个人中心页
    ├── settings_page.dart        # 设置页
    ├── splash_page.dart          # 启动页
    ├── video_call_page.dart      # 视频/语音通话页
    └── red_packet_page.dart      # 红包页
```

## 运行项目

### 环境要求
- Flutter SDK >= 3.11.0
- Dart SDK >= 3.11.0

### 安装依赖

```bash
flutter pub get
```

### 运行应用

```bash
# Windows
flutter run -d windows

# macOS
flutter run -d macos

# Web
flutter run -d chrome

# Android
flutter run -d android

# iOS
flutter run -d ios
```

### 构建发布版

```bash
# Windows
flutter build windows

# Android APK
flutter build apk

# iOS
flutter build ios

# Web
flutter build web
```

## 依赖包

| 包名 | 版本 | 用途 |
|------|------|------|
| flutter | SDK | Flutter 框架 |
| cupertino_icons | ^1.0.8 | iOS 风格图标 |

## 界面预览

应用采用微信的设计风格：
- 主题色：`#1AAD19`（微信绿）
- 背景色：`#EDEDED`（浅灰）
- 消息气泡：`#95EC69`（发送）、白色（接收）

## 开发说明

### 数据模拟
目前使用模拟数据，包括：
- 聊天列表数据
- 联系人数据
- 消息数据
- 朋友圈动态数据

### 扩展建议
1. 接入真实的 IM SDK（如 OpenIM）
2. 添加本地数据库存储
3. 实现用户认证系统
4. 添加推送通知功能
5. 支持多媒体消息（图片、视频、语音）

## 许可证

MIT License
