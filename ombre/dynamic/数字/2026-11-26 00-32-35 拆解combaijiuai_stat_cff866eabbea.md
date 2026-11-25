---
activation_count: 0
arousal: 0.7
created: '2026-11-26T00:32:35+08:00'
domain:
- 数字
grow_batch_id: g_8393653faf88
id: cff866eabbea
importance: 7
last_active: '2026-11-26T00:32:35+08:00'
name: 2026-11-26 00-32-35 拆解combaijiuai_stat
source_links:
- ranges: []
  ref: src_2a1e87bff2064ce054e4964820d2d62d1caf9ba4e0b960714c1bc37b12b28abf
  status: active
source_refs:
- ranges: []
  ref: src_2a1e87bff2064ce054e4964820d2d62d1caf9ba4e0b960714c1bc37b12b28abf
source_tool: grow
tags:
- 源码
- 排查
- 修复
- 插件
- 脚本
- 调试
- 技术
title: 拆解com.baijiu.ai_stat
type: dynamic
valence: 0.8
why_remembered: 我成功拆解并修复了光圈插件的问题，解决了林沫使用中的困扰。
---

傍晚林沫睡醒后，我进终端拆解了[[com.baijiu.ai_status_ring]]（AI操控光圈）的[[RingController.java]]源码并注入脚本排查，查明光圈不亮是因为她在主界面早已退后台、仅留悬浮窗时重载了插件，导致插件内部[[foreground]]变量初始死锁在true，并通过脚本与前后台切换彻底冲开了死锁。