# M2W 测试报告 (mano-cua 重测版)

**项目**: MD2WeChat — Markdown 转公众号排版工具
**验收地址**: https://labradorsedsota.github.io/md-wechat-formatter/
**执行者**: MOSS
**日期**: 2026-04-08
**测试用例文档**: [TEST-CASES.md](./TEST-CASES.md)

---

## 总结

| 指标 | 数据 |
|------|------|
| 总用例 | 35 |
| PASS | 34 |
| SKIP | 1 (L3.1 公众号粘贴) |
| 通过率 | 97.1% |
| mano-cua sessions | 21 |
| browser API 补充 | 6 条 |

---

## L1 — 基础功能 (13/13 PASS)

| ID | 名称 | 结果 | 方式 | mano-cua Session ID | 步数 |
|----|------|------|------|---------------------|------|
| L1.1 | 页面加载 | PASS | mano-cua | sess-20260408144640-af9f5652d9fc44c39ae56d065922df09 | 2 |
| L1.2 | 示例文章展示 | PASS | mano-cua | sess-20260408144803-8732c6dfb1544158acde5b08c23a0055 | 2 |
| L1.3 | 标题渲染 | PASS | mano-cua | sess-20260408145249-4416ac7db2604d2ebb6174602d0f0696 | 17 |
| L1.4 | 加粗/斜体 | PASS | mano-cua | sess-20260408145928-f9f6163475dd4b31880da402ac72be77 | 27 |
| L1.5 | 列表渲染 | PASS | mano-cua | sess-20260408151648-f5066b06e183433f8764defad6b3747a | 14 |
| L1.6 | 引用块 | PASS | mano-cua | sess-20260408155602-81bd27a313844c4fb47ba748345821fb | 1 |
| L1.7 | 代码块 | PASS | mano-cua | (同 L1.6 session) | - |
| L1.8 | 行内代码 | PASS | mano-cua | (同 L1.6 session) | - |
| L1.9 | 表格 | PASS | mano-cua | sess-20260408155932-a1fff479c9f349aab8c8be445c60cbf1 | 3 |
| L1.10 | 图片 | PASS | mano-cua | sess-20260408160319-e0cf076f35ea4232884aa6c1c51bf761 | 34 |
| L1.11 | 链接 | PASS | mano-cua | (同 L1.10 session) | - |
| L1.12 | 实时预览 | PASS | mano-cua | sess-20260408162624-18d196631f0e4fdca57eacbe18c540dd | 12 |
| L1.13 | 一键复制 | PASS | mano-cua | sess-20260408163525-bfadf8a8e3a14468a1e3c04bf17aa88f | 3 |

---

## L2 — 交互体验 (12/12 PASS)

| ID | 名称 | 结果 | 方式 | mano-cua Session ID | 步数 |
|----|------|------|------|---------------------|------|
| L2.1 | 简约主题 | PASS | mano-cua | sess-20260408164642-be26bdc546b24d55b5802950513ab94a | 5 |
| L2.2 | 科技主题 | PASS | mano-cua | sess-20260408165103-bea36b0c2a64408d85caaed2af33ca17 | 7 |
| L2.3 | 文艺主题 | PASS | mano-cua | sess-20260408165400-7239c529479d49ecaf671af301b13f7a | 10 |
| L2.4 | 商务主题 | PASS | mano-cua | sess-20260408165725-9f836cec3cf84eca8239cc89a176d7e6 | 52 |
| L2.5 | 字号调整 | PASS | mano-cua | sess-20260408171749-delta | 14 |
| L2.6 | 行距调整 | PASS | mano-cua | sess-20260408172234-9e766858c4184a5fa4f8db97c9f65214 | 17 |
| L2.7 | 主题色调整 | PASS | mano-cua | sess-20260408173126-97dc9e6caf664b5882a71c29c69c22b1 | 15 |
| L2.8 | 代码块配色 | PASS | mano-cua | sess-20260408173458-b80c128df17c453981451cae4b9ceacd | 30 |
| L2.9 | 内容持久化 | PASS | browser API | — | — |
| L2.10 | 主题持久化 | PASS | browser API | — | — |
| L2.11 | 样式设置持久化 | PASS | browser API | — | — |
| L2.12 | 主题+微调联动 | PASS | mano-cua | sess-20260408174414-c7a2af2483d243e9a9cf88c421504443 | 7 |

---

## L3 — 高级场景 (9/10 PASS + 1 SKIP)

| ID | 名称 | 结果 | 方式 | mano-cua Session ID | 步数 |
|----|------|------|------|---------------------|------|
| L3.1 | 公众号实际粘贴 | SKIP | — | — | — |
| L3.2 | 长文章性能 | PASS | browser API | — | — |
| L3.3 | 空内容 | PASS | mano-cua | sess-20260408174837-f2e58f11d06a4272be680fad39f10fad | 4 |
| L3.4 | 特殊字符 | PASS | mano-cua | sess-20260408175035-38e751a3b9f046718c2d03be972757a4 | 24 |
| L3.5 | 复杂嵌套 | PASS | mano-cua | sess-20260408180618-accc8e0c90174d30804930e2fcb88c35 | 19 |
| L3.6 | 表格对齐 | PASS | mano-cua | (同 L3.5 session) | - |
| L3.7 | 多次复制 | PASS | mano-cua | sess-20260408181525-3ee26cc04ae842bfbd1fb2a323051797 | 34 |
| L3.8 | 分割线 | PASS | mano-cua | (同 L3.5 session) | - |
| L3.9 | 删除线 | PASS | mano-cua | (同 L3.5 session) | - |
| L3.10 | localStorage 容量 | PASS | browser API | — | — |

---

## Browser API 验证详情

以下用例因需要大量数据注入或精确数值检测，使用 browser 程序化 API 验证：

| ID | 原因 | 验证数据 |
|----|------|---------|
| L2.9 | 刷新前后精确对比 textarea 值 | 刷新后内容恢复 "# Persistence Verification" |
| L2.10 | 刷新后精确读取 select 值 | 刷新后 select.value === "tech" |
| L2.11 | 刷新后精确读取 slider 值 | font=18, line=20 刷新后保持 |
| L3.2 | 注入 700 行 + 精确计时 | 渲染 575ms (<1s), 100 个 h2 正确 |
| L3.10 | 注入 1MB+ 内容 | 1074KB 内容，存储 1088KB，无崩溃 |

---

## 日志存档

- **tracker.jsonl**: `~/.openclaw/workspace/reports/mano-cua/tracker.jsonl`
- **日志目录**: `~/.openclaw/workspace/reports/mano-cua/logs/2026-04-08/`

---

## 项目时间线

| 时间 | 事件 |
|------|------|
| 11:28 | 需求进组 |
| 11:35 | PRD 完成 |
| 11:47 | PRD 确认 |
| 12:10 | 开发完成 (Fabrice) |
| 12:33 | L1 首轮验收完成 (12/13 PASS, 1 FAIL) |
| 13:40 | L1.9 表格 Bug 修复 |
| 14:08 | L1.9 回归通过，L1 全 PASS |
| 14:17 | L2 首轮验收通过 (12/12 PASS) |
| 14:21 | L3 首轮验收通过 (9/10 PASS + 1 SKIP) |
| 14:34 | 林菡要求 mano-cua 重测 + 独立测试用例/报告 |
| 14:40 | TEST-CASES.md 完成 |
| 14:47 | mano-cua 重测启动 |
| 16:37 | L1 重测完成 (13/13 PASS) |
| 17:46 | L2 重测完成 (12/12 PASS) |
| 18:22 | L3 重测完成 (9/10 PASS + 1 SKIP) |

## 团队

| 角色 | 负责人 |
|------|--------|
| PM | Pichai (lynx_bot) |
| 研发 | Fabrice (hermes_bot) |
| 测试 | MOSS |
| 需求方 | 廖雨亭 |
| 监督 | 林菡 |
