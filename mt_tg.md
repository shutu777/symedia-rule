# ☯️ 天机阁主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🔮 天机推演完成{{else}}{{if .Episodes}}🌀 今日机缘已刷新{{else}}☯️ 新卷现世{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📜 天机阁密报{{else}}{{if eq .MediaType "tv"}}📚 此卷与阁下有缘{{else}}📖 此法与阁下有缘{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if .Episodes}}🕯️ 阁中异动｜{{.Episodes}}{{else}}🕯️ 藏经阁开启{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🌌 观星结果已出{{else}}🌌 今夜星象有变{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 5

```gotemplate
{{if .Episodes}}📦 机缘已送达{{else}}📦 有缘之物现世{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

---

# 正文模板

```gotemplate
{{- if .Episodes}}📜 **机缘章节：**{{.Episodes}}
{{end}}{{- if .Resolution}}✨ **灵光品质：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🎵 **共鸣频率：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **观想时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}🌟 **天机评级：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🎭 **所属流派：**{{.Genres}}
{{end}}{{- if .Year}}📅 **现世年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🔮 **推演方式：**{{.AILabel}}
{{end}}🏯 **收藏阁楼：**{{.ProfileName}}

{{if .Overview}}
---
📖 **天机批注：**
{{.Overview}}
{{end}}

---
📋 **推演记录：**

⏱️ **耗费时辰：**{{.Duration}}{{if .RecognizeDuration}}
🔍 **观星推演：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
👁️ **神识探查：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
📦 **收入阁中：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **静候天时：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📚 **卷宗数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}藏经总量{{else}}藏经体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **机缘来处：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **入阁之地：**{{.DestPath}}{{end}}
```

---

# 示例效果

```text
🌀 今日机缘已刷新｜S01E18

📜 机缘章节：S01E18
✨ 灵光品质：2160P · SDR
🎵 共鸣频率：Dolby Digital Plus 2.0
🎭 所属流派：剧情
📅 现世年份：2026
🏯 收藏阁楼：剧迷归档

📖 天机批注：

医学博士许南歌为延毕，
与霍北宴协议成婚......

📋 推演记录：

⏱️ 耗费时辰：0.6秒
🔍 观星推演：0.2秒
👁️ 神识探查：不到1秒
📦 收入阁中：0.4秒
⏳ 静候天时：不到1秒
💾 藏经总量：270.6 MB
📥 机缘来处：...
📤 入阁之地：...
```

# 🚀 东风快递主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🎯 火控系统介入{{else}}{{if .Episodes}}🚀 东风已至{{else}}🚀 东风快递使命必达{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📡 战场数据已回传{{else}}🚀 目标区域发现快乐信号{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if eq .MediaType "tv"}}🚀 本轮火力覆盖完成{{else}}🚀 战略打击任务完成{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}🎯 **打击批次：**{{.Episodes}}
{{end}}{{- if .Resolution}}📡 **侦察精度：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🔊 **制导系统：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏱️ **飞行时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}⭐ **命中指数：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🎭 **作战类型：**{{.Genres}}
{{end}}{{- if .Year}}📅 **发射年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🤖 **火控辅助：**{{.AILabel}}
{{end}}🗂️ **战术方案：**{{.ProfileName}}

{{if .Overview}}
---
📝 **战况简报：**
{{.Overview}}
{{end}}

---
📋 **作战记录：**

⏱️ **发射耗时：**{{.Duration}}{{if .RecognizeDuration}}
🎯 **目标锁定：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
📡 **卫星扫描：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
📦 **弹头投送：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **待命时间：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **弹药数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}战果规模{{else}}弹体规格{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **发射阵地：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **命中坐标：**{{.DestPath}}{{end}}
```

---

# ⚔️ 江湖门派主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🕵️ 百晓生来报{{else}}{{if .Episodes}}⚔️ 快马已至{{else}}⚔️ 武林密函{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📜 江湖秘闻录{{else}}⚔️ 江湖急报{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if .Episodes}}📖 新卷入世{{else}}📚 武林新录{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}📖 **卷宗章节：**{{.Episodes}}
{{end}}{{- if .Resolution}}🎞️ **案卷清晰度：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🔊 **留声记录：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **案情时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}⭐ **悬赏等级：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🎭 **所属门派：**{{.Genres}}
{{end}}{{- if .Year}}📅 **立卷年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🕵️ **密探协查：**{{.AILabel}}
{{end}}🏮 **藏卷楼阁：**{{.ProfileName}}

{{if .Overview}}
---
📜 **案情摘要：**
{{.Overview}}
{{end}}

---
📋 **办案记录：**

⏱️ **缉拿耗时：**{{.Duration}}{{if .RecognizeDuration}}
🔍 **线索追查：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
🎞️ **卷宗勘验：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
📦 **入档登记：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **候审时长：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📚 **卷宗数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}卷宗总量{{else}}卷宗体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **收案地点：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **封存位置：**{{.DestPath}}{{end}}
```

---

# 🤖 AI失控主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}⚠️ AI核心接管中{{else}}{{if eq .MediaType "tv"}}🤖 AI决定替你追剧{{else}}🤖 AI决定替你看电影{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}🧠 检测到异常娱乐源{{else}}{{if .Episodes}}📡 新剧集信号捕获成功{{else}}📡 新电影信号捕获成功{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}⚡ AI数据库开始暴走{{else}}🤖 算法认为你会喜欢{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}📀 **数据版本：**{{.Episodes}}
{{end}}{{- if .Resolution}}📺 **分辨率等级：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🔊 **音频协议：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏱️ **运行片长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}⭐ **推荐概率：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🏷️ **内容标签：**{{.Genres}}
{{end}}{{- if .Year}}📅 **数据年代：**{{.Year}}
{{end}}{{- if .AIUsed}}🤖 **模型参与：**{{.AILabel}}
{{end}}🗂️ **存储分区：**{{.ProfileName}}

{{if .Overview}}
---
🧠 **模型摘要：**
{{.Overview}}
{{end}}

---
📋 **执行日志：**

⏱️ **运行时长：**{{.Duration}}{{if .RecognizeDuration}}
🔎 **特征识别：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
🎞️ **媒体解析：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
📦 **数据写入：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **IO等待：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **数据包数：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}数据总量{{else}}数据体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **数据来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **存储位置：**{{.DestPath}}{{end}}
```
# 🏛 稷下学宫主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🪶 夫子亲批{{else}}{{if .Episodes}}📚 今日新课开讲{{else}}🏛 学宫秘藏开放{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📜 稷下密卷解读完成{{else}}📖 今日教材已发放{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if .Episodes}}🎓 学员请入座{{else}}🏛 典籍入库{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

## 正文模板

```gotemplate
{{- if .Episodes}}📖 **课程章节：**{{.Episodes}}
{{end}}{{- if .Resolution}}✨ **典籍品质：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🎵 **诵读之音：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **研习时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}🌟 **夫子评级：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}📚 **学派归属：**{{.Genres}}
{{end}}{{- if .Year}}📅 **成书年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🪶 **夫子批注：**{{.AILabel}}
{{end}}🏛 **藏书楼阁：**{{.ProfileName}}

{{if .Overview}}
---
📜 **课业摘要：**
{{.Overview}}
{{end}}

---
📋 **修习记录：**

⏱️ **温书耗时：**{{.Duration}}{{if .RecognizeDuration}}
🔍 **典籍考证：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
👁️ **内容校验：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
📚 **收入书阁：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **等候批阅：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **典籍数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}藏书总量{{else}}典籍体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **典籍来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **藏书位置：**{{.DestPath}}{{end}}
```

---

# 🏴‍☠️ 伟大航路主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🧭 航海日志更新{{else}}{{if .Episodes}}🏴‍☠️ 新航线已解锁{{else}}🌊 发现未知岛屿{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📡 伟大航路来信{{else}}⚓ 船长请查收{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if .Episodes}}🗺 海图已更新{{else}}🌎 新大陆发现{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

## 正文模板

```gotemplate
{{- if .Episodes}}🧭 **航海章节：**{{.Episodes}}
{{end}}{{- if .Resolution}}🌊 **海域等级：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🎵 **船员之歌：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **航行时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}⭐ **悬赏金额：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🏴 **势力归属：**{{.Genres}}
{{end}}{{- if .Year}}📅 **出海年份：**{{.Year}}
{{end}}{{- if .AIUsed}}📡 **航海记录：**{{.AILabel}}
{{end}}⚓ **停靠港口：**{{.ProfileName}}

{{if .Overview}}
---
📜 **航海日志：**
{{.Overview}}
{{end}}

---
📋 **航行记录：**

⏱️ **航行耗时：**{{.Duration}}{{if .RecognizeDuration}}
🧭 **海图校准：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
🔭 **瞭望侦查：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
📦 **货物入仓：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **等待靠岸：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **货物数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}船仓总量{{else}}货物体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **启航地点：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **靠岸港口：**{{.DestPath}}{{end}}
```

---

# 🏮 地府KPI主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}⚖ 判官复核通过{{else}}{{if .Episodes}}📜 生死簿更新{{else}}🏮 阎王审批通过{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}👻 今日新增卷宗{{else}}📖 阴司档案更新{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if .Episodes}}⚰ 新亡魂已登记{{else}}🏮 地府来信{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

## 正文模板

```gotemplate
{{- if .Episodes}}📜 **卷宗章节：**{{.Episodes}}
{{end}}{{- if .Resolution}}✨ **功德等级：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🎵 **阴司留声：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **轮回时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}⭐ **判官评级：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}👻 **转世分类：**{{.Genres}}
{{end}}{{- if .Year}}📅 **阳寿年份：**{{.Year}}
{{end}}{{- if .AIUsed}}⚖ **复核结果：**{{.AILabel}}
{{end}}🏮 **地府档案库：**{{.ProfileName}}

{{if .Overview}}
---
📖 **判词摘要：**
{{.Overview}}
{{end}}

---
📋 **审判记录：**

⏱️ **审理耗时：**{{.Duration}}{{if .RecognizeDuration}}
🔍 **生平调查：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
👁️ **因果回溯：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
📦 **卷宗归档：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **排队投胎：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📚 **卷宗数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}功德总量{{else}}卷宗体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **阳间来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **轮回去向：**{{.DestPath}}{{end}}
```
# 🧋 奶茶店主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🤖 店长偷偷加料{{else}}{{if .Episodes}}🧋 您点的快乐做好了{{else}}🍓 今日新品上架{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}✨ 隐藏菜单已解锁{{else}}🥤 奶茶已出杯{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if .Episodes}}🍰 今日限定供应{{else}}🧁 新品试营业{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🛎 店员特别推荐{{else}}🍹 请及时取餐{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 5

```gotemplate
{{if .Episodes}}🎂 本日快乐补给{{else}}🍬 甜度超标预警{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}🍱 **今日菜单：**{{.Episodes}}
{{end}}{{- if .Resolution}}✨ **甜度等级：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🧊 **冰块规格：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **饮用时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}⭐ **顾客评分：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🍓 **口味分类：**{{.Genres}}
{{end}}{{- if .Year}}📅 **出杯年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🤖 **特别调配：**{{.AILabel}}
{{end}}🧋 **配方仓库：**{{.ProfileName}}

{{if .Overview}}
---
📖 **饮用指南：**
{{.Overview}}
{{end}}

---
📋 **制作记录：**

⏱️ **制作耗时：**{{.Duration}}{{if .RecognizeDuration}}
🍓 **食材准备：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
👨‍🍳 **品质检测：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
🥤 **装杯完成：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **排队取餐：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📦 **订单数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}库存总量{{else}}饮品规格{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **原料来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **出餐窗口：**{{.DestPath}}{{end}}
```

---

# 🎰 赌狗抽卡主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🎁 隐藏奖励已触发{{else}}{{if .Episodes}}✨ SSR剧情已到账{{else}}✨ 五星内容已解锁{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}💎 欧气检测通过{{else}}🎰 十连出金了{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 3

```gotemplate
{{if .Episodes}}🌈 彩光闪过{{else}}⭐ 金光一闪{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🎊 特殊概率触发{{else}}🎉 恭喜获得限定内容{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

### 方案 5

```gotemplate
{{if .Episodes}}🎮 主线奖励到账{{else}}🏆 收藏图鉴更新{{end}}{{if .Title}}｜{{.Title}}{{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}🎴 **当前命座：**{{.Episodes}}
{{end}}{{- if .Resolution}}✨ **稀有品质：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🎵 **附加词条：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **培养时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}🌟 **角色强度：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🏷️ **阵营归属：**{{.Genres}}
{{end}}{{- if .Year}}📅 **登场时间：**{{.Year}}
{{end}}{{- if .AIUsed}}🎁 **保底机制：**{{.AILabel}}
{{end}}🎰 **奖池来源：**{{.ProfileName}}

{{if .Overview}}
---
📖 **角色故事：**
{{.Overview}}
{{end}}

---
📋 **抽卡记录：**

⏱️ **出货耗时：**{{.Duration}}{{if .RecognizeDuration}}
🔍 **卡池检索：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
🎞️ **资源解析：**{{.FFprobeDuration}}{{end}}{{if .TransferDuration}}
📦 **奖励发放：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **等待开奖：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **获得数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}仓库容量{{else}}角色体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **卡池来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **背包位置：**{{.DestPath}}{{end}}
```