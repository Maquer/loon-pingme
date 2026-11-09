# PingMe 自动签到+视频奖励 - Loon 插件

## 简介
Loon 插件，PingMe App 每日自动签到 + 看视频领币，支持多账号。

## 快速开始（Loon 网络导入）
在 Loon 中点「网络导入」，粘贴插件 URL：
```
https://cdn.jsdelivr.net/gh/Maquer/loon-pingme@main/PingMe.loon.js
```

> 若你的 Loon 版本不支持 script-url，回退方案见文末。

## 使用
1. **开启 MITM + 信任证书**：Loon → MITM 开开关 → 装证书 → iOS 设置 → 通用 → 关于本机 → 证书信任设置 → 信任 Loon
2. **抓一次包**：打开 PingMe App，触发余额接口 → 弹「✅ 新账号已入库」
3. **自动/手动运行**：每天 8:20/20:20 自动签到；或 Loon 脚本列表手动点运行验证

## 排查
- 没收到通知 → 检查 MITM 是否开、证书是否信任、iPhone 是否连 Loon 代理
- 抓不到账号 → 需先打开 PingMe App 触发 queryBalanceAndBonus

## 回退（不支持 script-url 时）
1. 下载脚本：`https://cdn.jsdelivr.net/gh/Maquer/loon-pingme@main/PingMe.loon.js`，存到 Loon 脚本目录
2. 导入插件：`https://cdn.jsdelivr.net/gh/Maquer/loon-pingme@main/PingMe.plugin`

Created by 小蒋 | 2026-11-09
