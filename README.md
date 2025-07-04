# Job Track App 产品需求文档（PRD v2）

## 一、产品简介

Job Track 是一款面向「转型期/职场早期用户」的 **智能求职记录与成长辅助工具**。用户可以通过本产品：
- 管理自己的岗位投递记录
- 统计投递与面试阶段的数据趋势
- 自动解析岗位信息
- 获取模拟面试支持与心理调节建议
- 联动其他成长型

目标用户：
- 校招用户
- 职业转型者
- 毕业1-5年职场人
- 期望系统整理、评估自己求职成果并保持心态稳定的用户

---

## 二、产品结构

### 1. 首页（Dashboard）

#### 功能模块：
- 🔗 岗位投递方框解析区：
  - 支持粘贴 JD 文本或岗位链接
  - 一键提取：公司、岗位名、平台、地点、关键词、分类标签

- 📊 投递数据概览区：
  - 本周/月 投递趋势折线图
  - 面试阶段计数（已投递/约面试/Offer/淘汰）
  - 高亮显示：下周重要事项

- 🕓 快速入口：
  - 添加新岗位
  - 设置提醒
  - 导入/导出数据

---

### 2. 投递记录页（Record Detail）

#### 功能模块：
- 岗位信息卡片或表格：
  - 字段：岗位名、公司、时间、关键词、行业、地点、备注、阶段、标签
- 支持功能：
  - 添加/编辑/删除岗位记录
  - 自定义标签（如梦中情岗、通投岗等）
  - 阶段标记：已投递、HR看过、约面试、二面、Offer 等
  - 数据导出（PDF/Excel）
  - 快捷筛选排序（按阶段/岗位类型等）

---

### 3. 我的（Profile）

#### 功能模块：
- 基本资料（可选）
- 我的偏好岗位标签
- 数据分析视图（饼图 + 柱状图）
- 提醒设置
- App 联动入口（Her Sense / 中药查询）
- 彩虹卡鼓励模块（每日一句 + 深呼吸训练）

---

## 三、扩展功能模块（阶段二）

### ✅ 1. AI 模拟面试支持（内测版）

- 基于岗位 JD + 用户输入简历内容，自动生成 3~5 个常见面试问题
- 用户可录音回答 / 文本输入
- 系统给出反馈：
  - 关键词使用分析
  - 逻辑清晰度打分
  - 提升建议

### ✅ 2. OfferShow 数据接入（Beta）

- 用户输入岗位关键词或链接，自动查询近似 Offer 数据
- 可视化展示：
  - 经验/学历对应薪资范围
  - 不同地区对比

### ✅ 3. 心态调节辅助系统

- 面试前彩虹卡抽签：随机正向语句（Her Sense 联动）
- 三分钟情绪调节：音频/呼吸练习
- 情绪记录日志：每日一问（今天你为求职做了什么？你感觉如何？）

---

## 四、技术架构简要

- **前端**：React Native + Expo + Tailwind CSS 适配
- **数据管理**：本地 JSON（初版） → Firebase / Supabase（进阶版）
- **AI 模块**：调用 Gemini / GPT API 完成内容生成与分析
- **日程提醒**：接入 iOS/Android 系统日历 or 微信推送

---

## 五、里程碑计划建议（可选）

| 时间 | 目标 |
|------|------|
| 第1周 | 完成首页岗位解析 & 添加模块开发 |
| 第2周 | 实现投递详情页及筛选功能 |
| 第3周 | 完成数据可视化折线图/饼图 |
| 第4周 | 集成 AI 模拟面试功能（测试版） |
| 第5周+ | 打磨 UI 细节，准备发布至平台 |

---

## 六、命名建议 & slogan

> Job Track – 智能记录 · 平稳前行  
> 「不再焦虑的求职路，从今天开始」

---

