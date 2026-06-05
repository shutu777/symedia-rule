# TG 通知主题模板合集 v2

## 目录

- [☯️ 天机阁主题](#tianjige)
- [🧋 奶茶店主题](#naicha)
- [🏛 稷下学宫主题](#jixia)
- [🤖 AI失控主题](#ai)
- [🪩 赛博夜市主题](#cyber-night-market)
- [🛸 外星人偷看地球主题](#alien-earth)
- [🎤 宇宙KTV主题](#cosmic-ktv)
- [🚀 东风快递主题](#dongfeng)
- [⚔️ 江湖门派主题](#jianghu)
- [🏴‍☠️ 伟大航路主题](#hanglu)
- [🎰 赌狗抽卡主题](#chouka)
- [🧃 便利店夜班主题](#night-shift-store)

---
<a id="tianjige"></a>

# ☯️ 天机阁主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🔮 天机推演完成{{else}}{{if .Episodes}}🌀 今日机缘已刷新{{else}}☯️ 新卷现世{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📜 天机阁密报{{else}}{{if eq .MediaType "tv"}}📚 此卷与阁下有缘{{else}}📖 此法与阁下有缘{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🌌 天机再动{{else}}{{if .Episodes}}🕯️ 阁中异动{{else}}🕯️ 藏经阁开启{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🌌 观星结果已出{{else}}{{if eq .MediaType "tv"}}🌌 今夜星象有变{{else}}🌌 星盘照见新卷{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🔮 机缘由天机推送{{else}}{{if .Episodes}}📦 机缘已送达{{else}}📦 有缘之物现世{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
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
👁️ **神识探查：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
📦 **收入阁中：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **静候天时：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📚 **卷宗数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}藏经总量{{else}}藏经体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **机缘来处：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **入阁之地：**{{.DestPath}}{{end}}
```

---

<a id="naicha"></a>

# 🧋 奶茶店主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🤖 店长偷偷加料{{else}}{{if .Episodes}}🧋 您点的快乐做好了{{else}}🍓 今日新品上架{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}✨ 隐藏菜单已解锁{{else}}{{if .Episodes}}🥤 本杯加更已出杯{{else}}🥤 奶茶已出杯{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🛎 店员偷偷推荐{{else}}{{if .Episodes}}🍰 今日限定供应{{else}}🧁 新品试营业{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🛎 店员特别推荐{{else}}{{if eq .MediaType "tv"}}🍹 追剧奶茶请及时取餐{{else}}🍹 观影奶茶请及时取餐{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🤖 店长判定值得加料{{else}}{{if .Episodes}}🎂 本日快乐补给{{else}}🍬 甜度超标预警{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
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
👨‍🍳 **品质检测：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
🥤 **装杯完成：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **排队取餐：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📦 **订单数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}库存总量{{else}}饮品规格{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **原料来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **出餐窗口：**{{.DestPath}}{{end}}
```

---

<a id="jixia"></a>

# 🏛 稷下学宫主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🪶 夫子亲批{{else}}{{if .Episodes}}📚 今日新课开讲{{else}}🏛 学宫秘藏开放{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📜 稷下密卷解读完成{{else}}{{if .Episodes}}📖 今日教材已发放{{else}}📖 镇馆典籍已发放{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🪶 夫子加急批阅{{else}}{{if .Episodes}}🎓 学员请入座{{else}}🏛 典籍入库{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🧠 稷下机关术已验算{{else}}{{if .Episodes}}🪶 夫子点名，新课开卷{{else}}🪶 夫子点名，典籍入阁{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}📚 学宫智库完成补全{{else}}{{if eq .MediaType "tv"}}🎓 今日课业请及时研习{{else}}🎓 今日典籍请及时研习{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
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
👁️ **内容校验：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
📚 **收入书阁：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **等候批阅：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **典籍数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}藏书总量{{else}}典籍体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **典籍来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **藏书位置：**{{.DestPath}}{{end}}
```

---

<a id="ai"></a>

# 🤖 AI失控主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}⚠️ AI核心接管中{{else}}{{if eq .MediaType "tv"}}🤖 AI决定替你追剧{{else}}🤖 AI决定替你看电影{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}🧠 检测到异常娱乐源{{else}}{{if .Episodes}}📡 新剧集信号捕获成功{{else}}📡 新电影信号捕获成功{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}⚡ AI数据库开始暴走{{else}}{{if eq .MediaType "tv"}}🤖 算法认为你会追下去{{else}}🤖 算法认为你会喜欢{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

---

### 方案 4

```gotemplate
{{if .AIUsed}}🧬 模型自我进化完成{{else}}{{if .Episodes}}📡 新一集快乐样本入库{{else}}📡 新电影快乐样本入库{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}⚠️ 人类娱乐计划升级{{else}}{{if eq .MediaType "tv"}}🤖 检测到高浓度电子榨菜{{else}}🤖 检测到高价值观影样本{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```


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
🎞️ **媒体解析：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
📦 **数据写入：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **IO等待：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **数据包数：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}数据总量{{else}}数据体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **数据来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **存储位置：**{{.DestPath}}{{end}}
```

---

<a id="cyber-night-market"></a>

# 🪩 赛博夜市主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🪩 夜市AI掌勺完成{{else}}{{if .Episodes}}🌃 霓虹摊位上新一串{{else}}🪩 赛博夜市开摊啦{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}🤖 电子摊主已验货{{else}}{{if .Episodes}}🍢 新一串快乐出炉{{else}}🌆 今日夜市灯牌亮起{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🧠 霓虹菜单自动更新{{else}}{{if eq .MediaType "tv"}}🪩 追剧摊位开始营业{{else}}🪩 观影摊位开始营业{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}⚡ 赛博厨师加急出餐{{else}}{{if .Episodes}}🌭 本摊新章已装袋{{else}}🍜 本摊新品已上桌{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🪩 AI试吃员给出好评{{else}}{{if .Episodes}}🍡 夜市加更小串已到{{else}}🌃 霓虹快乐补货完成{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}🍢 **夜市摊号：**{{.Episodes}}
{{end}}{{- if .Resolution}}💡 **霓虹亮度：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🔊 **摊位音响：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **逛摊时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}🌟 **人气指数：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🌶️ **摊位口味：**{{.Genres}}
{{end}}{{- if .Year}}📅 **开摊年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🤖 **电子掌勺：**{{.AILabel}}
{{end}}🏮 **夜市档口：**{{.ProfileName}}

{{if .Overview}}
---
📋 **今日招牌：**
{{.Overview}}
{{end}}

---
🧾 **出摊记录：**

⏱️ **开摊耗时：**{{.Duration}}{{if .RecognizeDuration}}
📱 **扫码识别：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
💡 **灯牌巡检：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
🥡 **装袋出摊：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **排队时间：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
🍢 **货品数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}摊位库存{{else}}单品份量{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **进货来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **摆摊位置：**{{.DestPath}}{{end}}
```

---

<a id="alien-earth"></a>

# 🛸 外星人偷看地球主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🛸 外星智脑完成分析{{else}}{{if .Episodes}}👽 地球连续剧样本+1{{else}}🛸 地球娱乐样本捕获{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}🧠 母舰分析报告出炉{{else}}{{if .Episodes}}📡 人类追更行为被记录{{else}}📡 人类观影行为被记录{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}👽 外星观察员加急标注{{else}}{{if eq .MediaType "tv"}}🛸 发现可疑地球剧集{{else}}🛸 发现可疑地球电影{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🛰 轨道探针完成复核{{else}}{{if .Episodes}}👾 地球样本正在连载{{else}}👾 地球样本已打包{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🛸 外星AI表示想继续看{{else}}{{if .Episodes}}👽 观察员偷看了新一集{{else}}👽 观察员偷看了一整部{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}🧬 **样本编号：**{{.Episodes}}
{{end}}{{- if .Resolution}}🔭 **观测清晰度：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}📡 **地球声波：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **观察时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}⭐ **研究价值：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🏷️ **人类分类：**{{.Genres}}
{{end}}{{- if .Year}}📅 **地球年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🧠 **智脑判断：**{{.AILabel}}
{{end}}🛸 **母舰仓库：**{{.ProfileName}}

{{if .Overview}}
---
📝 **观测笔记：**
{{.Overview}}
{{end}}

---
📋 **偷看记录：**

⏱️ **捕获耗时：**{{.Duration}}{{if .RecognizeDuration}}
👽 **物种识别：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
🛰 **信号扫描：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
📦 **样本封存：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **母舰等待：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
🧪 **样本数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}样本总量{{else}}样本体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **信号来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **飞船仓位：**{{.DestPath}}{{end}}
```

---

<a id="cosmic-ktv"></a>

# 🎤 宇宙KTV主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🎤 AI调音师已上线{{else}}{{if .Episodes}}🎶 新歌已加入歌单{{else}}🎤 宇宙KTV开唱啦{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}🪩 自动混响调到满格{{else}}{{if .Episodes}}🎵 下一首已经排上{{else}}🎤 今晚主打歌已点好{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🤖 机械DJ完成切歌{{else}}{{if eq .MediaType "tv"}}🎧 追剧包厢开始合唱{{else}}🎧 观影包厢开始合唱{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🎛 银河音控完成校准{{else}}{{if .Episodes}}🌌 星河歌单更新一首{{else}}🌌 星河歌单加入新曲{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🎤 AI说这首必须唱{{else}}{{if .Episodes}}🪩 包厢屏幕跳出新章{{else}}🪩 包厢屏幕跳出新片{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}🎼 **点歌编号：**{{.Episodes}}
{{end}}{{- if .Resolution}}💡 **舞台灯光：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}🎙️ **麦克风配置：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **演唱时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}🔊 **全场分贝：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🎶 **曲风分类：**{{.Genres}}
{{end}}{{- if .Year}}📅 **发行年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🤖 **调音结果：**{{.AILabel}}
{{end}}🎤 **包厢曲库：**{{.ProfileName}}

{{if .Overview}}
---
📖 **歌曲介绍：**
{{.Overview}}
{{end}}

---
📋 **演唱记录：**

⏱️ **开唱耗时：**{{.Duration}}{{if .RecognizeDuration}}
🔍 **曲库检索：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
🎛️ **音轨校准：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
🎵 **加入歌单：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **等待切歌：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📀 **曲目数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}曲库容量{{else}}单曲大小{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **点歌来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **包厢位置：**{{.DestPath}}{{end}}
```

---

<a id="dongfeng"></a>

# 🚀 东风快递主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🎯 火控系统介入{{else}}{{if .Episodes}}🚀 东风已至{{else}}🚀 东风快递使命必达{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📡 战场数据已回传{{else}}{{if .Episodes}}🚀 目标区域发现剧集信号{{else}}🚀 目标区域发现快乐信号{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🎯 火控校准完毕{{else}}{{if eq .MediaType "tv"}}🚀 本轮火力覆盖完成{{else}}🚀 战略打击任务完成{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

---

### 方案 4

```gotemplate
{{if .AIUsed}}🛰 卫星制导已上线{{else}}{{if .Episodes}}🚀 新一轮精准投送{{else}}🚀 观众同志请立即接收{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🎯 智能火控锁定目标{{else}}{{if eq .MediaType "tv"}}🚀 该看的剧，一集没跑掉{{else}}🚀 该看的片，一部没跑掉{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```


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
📡 **卫星扫描：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
📦 **弹头投送：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **待命时间：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **弹药数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}战果规模{{else}}弹体规格{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **发射阵地：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **命中坐标：**{{.DestPath}}{{end}}
```

---

<a id="jianghu"></a>

# ⚔️ 江湖门派主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🕵️ 百晓生来报{{else}}{{if .Episodes}}⚔️ 快马已至{{else}}⚔️ 武林密函{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📜 江湖秘闻录{{else}}{{if .Episodes}}⚔️ 江湖急报，新回已至{{else}}⚔️ 江湖急报，名作入世{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🕵️ 百晓生已校录{{else}}{{if .Episodes}}📖 新卷入世{{else}}📚 武林新录{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

---

### 方案 4

```gotemplate
{{if .AIUsed}}🕵️ 暗探飞书已至{{else}}{{if .Episodes}}🐎 快马加鞭送新章{{else}}📜 武林帖已送达{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}📖 百晓生重新排榜{{else}}{{if eq .MediaType "tv"}}⚔️ 少侠，追更了{{else}}⚔️ 少侠，此片可观{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```


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
🎞️ **卷宗勘验：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
📦 **入档登记：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **候审时长：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📚 **卷宗数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}卷宗总量{{else}}卷宗体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **收案地点：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **封存位置：**{{.DestPath}}{{end}}
```

---

<a id="hanglu"></a>

# 🏴‍☠️ 伟大航路主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🧭 航海日志更新{{else}}{{if .Episodes}}🏴‍☠️ 新航线已解锁{{else}}🌊 发现未知岛屿{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}📡 伟大航路来信{{else}}{{if .Episodes}}⚓ 船长请查收，新航段抵达{{else}}⚓ 船长请查收，新宝藏入舱{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🧭 记录指针已校准{{else}}{{if .Episodes}}🗺 海图已更新{{else}}🌎 新大陆发现{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🔭 瞭望手发现异常航迹{{else}}{{if .Episodes}}🏴‍☠️ 新航段已抵达{{else}}🏴‍☠️ 新宝藏已入舱{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🧭 记录指针疯狂转动{{else}}{{if eq .MediaType "tv"}}⚓ 船员集合，继续追航{{else}}⚓ 船员集合，准备观影{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
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
🔭 **瞭望侦查：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
📦 **货物入仓：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **等待靠岸：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **货物数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}船仓总量{{else}}货物体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **启航地点：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **靠岸港口：**{{.DestPath}}{{end}}
```

---

<a id="chouka"></a>

# 🎰 赌狗抽卡主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🎁 隐藏奖励已触发{{else}}{{if .Episodes}}✨ SSR剧情已到账{{else}}✨ 五星内容已解锁{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}💎 欧气检测通过{{else}}{{if .Episodes}}🎰 单抽出金，新章到账{{else}}🎰 十连出金了{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🎲 概率被AI改写{{else}}{{if .Episodes}}🌈 彩光闪过{{else}}⭐ 金光一闪{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🎊 特殊概率触发{{else}}{{if eq .MediaType "tv"}}🎉 恭喜获得限定剧情{{else}}🎉 恭喜获得限定内容{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🎁 隐藏保底已触发{{else}}{{if .Episodes}}🎮 主线奖励到账{{else}}🏆 收藏图鉴更新{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
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
🎞️ **资源解析：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
📦 **奖励发放：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **等待开奖：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
📄 **获得数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}仓库容量{{else}}角色体积{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **卡池来源：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **背包位置：**{{.DestPath}}{{end}}
```

---

<a id="night-shift-store"></a>

# 🧃 便利店夜班主题（最终版）

## 标题模板

### 方案 1（推荐）

```gotemplate
{{if .AIUsed}}🧃 夜班店员智能盘货{{else}}{{if .Episodes}}🏪 夜班补货，新一集到架{{else}}🧃 便利店新品已上架{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 2

```gotemplate
{{if .AIUsed}}🤖 自助收银机完成推荐{{else}}{{if .Episodes}}🥪 凌晨货架补上新章{{else}}🏪 凌晨货架补上新品{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 3

```gotemplate
{{if .AIUsed}}🧾 小票机吐出神秘建议{{else}}{{if eq .MediaType "tv"}}🧃 追剧套餐已入冷柜{{else}}🧃 观影套餐已入冷柜{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 4

```gotemplate
{{if .AIUsed}}🏪 夜班系统偷偷加购{{else}}{{if .Episodes}}🍙 新一集已贴好价签{{else}}🍙 新品已贴好价签{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Episodes}} {{.Episodes}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

### 方案 5

```gotemplate
{{if .AIUsed}}🧃 店员说这个值得带走{{else}}{{if .Episodes}}🥤 深夜快乐补货完成{{else}}🥤 深夜快乐到货提醒{{end}}{{end}}{{if .Title}}｜{{.Title}}{{end}}{{if .Year}} ({{.Year}}){{end}}
```

---

## 正文模板

```gotemplate
{{- if .Episodes}}🏷️ **货架批次：**{{.Episodes}}
{{end}}{{- if .Resolution}}📦 **商品规格：**{{.Resolution}}{{if .DynamicRange}} · {{.DynamicRange}}{{end}}
{{end}}{{- if .AudioFormat}}📢 **店内广播：**{{.AudioFormat}}
{{end}}{{- if .VideoDuration}}⏳ **营业时长：**{{.VideoDuration}}
{{end}}{{- if .Rating}}⭐ **顾客评分：**{{printf "%.1f" .Rating}}/10
{{end}}{{- if .Genres}}🗂️ **货架分区：**{{.Genres}}
{{end}}{{- if .Year}}📅 **到货年份：**{{.Year}}
{{end}}{{- if .AIUsed}}🤖 **夜班推荐：**{{.AILabel}}
{{end}}🏪 **门店仓库：**{{.ProfileName}}

{{if .Overview}}
---
🧾 **商品说明：**
{{.Overview}}
{{end}}

---
📋 **夜班记录：**

⏱️ **上架耗时：**{{.Duration}}{{if .RecognizeDuration}}
🔍 **条码扫描：**{{.RecognizeDuration}}{{end}}{{if .FFprobeDuration}}
📦 **库存盘点：**{{.FFprobeDuration}}{{if .FFprobeCount}}（{{.FFprobeCount}}次）{{end}}{{end}}{{if .PrepareDuration}}
🛒 **入库摆放：**{{.TransferDuration}}{{end}}{{if .WaitDuration}}
⏳ **排队结账：**{{.WaitDuration}}{{end}}{{if gt .FileCount 1}}
🥤 **商品数量：**{{.FileCount}}{{end}}{{if .FileSize}}
💾 **{{if eq .MediaType "tv"}}货架容量{{else}}商品份量{{end}}：**{{.FileSize}}{{end}}{{if .SrcPath}}
📥 **进货渠道：**{{.SrcPath}}{{end}}{{if .DestPath}}
📤 **货架位置：**{{.DestPath}}{{end}}
```
