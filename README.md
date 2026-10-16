# 副业冷静室｜先聊明白，再掏钱

刷到别人的副业收入截图，准备买课、囤货、做账号之前，先把想法带来聊一遍。

这是一个可供 AI agent 加载的中文 skill，帮助你理清副业的真实条件：谁会付钱、自己缺什么能力、时间是否够用、每单能留下多少，以及最坏结果是否承担得起。

**劝退不是目的，但“有人成功”也不是值得你投入的理由。**

## 它会怎么帮你

- 面对“零基础＋AI＋轻松赚钱”，主动查行业资料，先给冷静判断，再问你的经验与条件。
- 拆开审美、内容生产、获客、交付与赚钱，识别工具之外的专业门槛。
- 核查资金来源与可承受损失，提醒借款、囤货及辞职风险。
- 用完整任务计时，检查“每天一小时”的预期是否现实。
- 比较副业与主业提升、求职转岗的机会成本，该停就停；值得验证时才设计小实验。

覆盖自媒体、带货、跨境、独立站、小众品牌、AI内容、技能接单、数字产品等方向。

## 一句话让 AI 帮你安装（推荐）

在具有联网和本地文件操作能力的 Codex 或其他 AI agent 中，直接发送：

```text
请帮我安装“副业冷静室”技能：
https://github.com/andypan555-ship-it/side-business-reality-check
请读取仓库说明，将完整技能文件夹（SKILL.md 和 references/）安装到当前 agent 支持的个人技能目录，文件夹名为 side-business-reality-check。
先确认当前工具和版本支持的技能路径，不覆盖已有同名技能。安装后核验文件完整性，告诉我实际安装位置和调用方法。若当前工具没有安装能力，请明确说明，不要只阅读文件就声称安装成功。
```

**Codex 也可以直接调用内置安装器：**

```text
$skill-installer 请从 https://github.com/andypan555-ship-it/side-business-reality-check 安装根目录技能，名称为 side-business-reality-check。
```

安装过程中，工具可能请求联网或技能目录写入权限，需要按实际提示授权。本技能本身不要求安装 Python、Node.js 或付费软件；agent 的使用费用与联网权限取决于你所用的产品。

## 终端安装（已安装 Git 的用户）

以下是本机个人技能安装，不适用于没有本地文件能力的网页聊天或云会话。只选当前工具对应的一组命令。目录已存在时 `git clone` 会停止，不要直接删除原目录。

### Codex

当前官方文档的个人技能目录为 `~/.agents/skills/`。旧版本或内置安装器可能使用不同目录，以当前工具核验结果为准；同一技能不要同时装到多个目录。

**macOS / Linux（终端）：**

```bash
mkdir -p "$HOME/.agents/skills"
git clone https://github.com/andypan555-ship-it/side-business-reality-check.git "$HOME/.agents/skills/side-business-reality-check"
```

**Windows（PowerShell）：**

```powershell
New-Item -ItemType Directory -Force -Path "$HOME/.agents/skills" | Out-Null
git clone https://github.com/andypan555-ship-it/side-business-reality-check.git "$HOME/.agents/skills/side-business-reality-check"
```

安装后在 Codex 输入：

```text
$side-business-reality-check 我想做AI漫剧赚钱，请先帮我了解行业现实，再判断我的条件。
```

Codex 会自动发现技能变化；未出现时重启 Codex，再用技能选择器或 `$` 查找。

### Claude Code（本地）

**macOS / Linux（终端）：**

```bash
mkdir -p "$HOME/.claude/skills"
git clone https://github.com/andypan555-ship-it/side-business-reality-check.git "$HOME/.claude/skills/side-business-reality-check"
```

**Windows（PowerShell）：**

```powershell
New-Item -ItemType Directory -Force -Path "$HOME/.claude/skills" | Out-Null
git clone https://github.com/andypan555-ship-it/side-business-reality-check.git "$HOME/.claude/skills/side-business-reality-check"
```

安装后在 Claude Code 输入：

```text
/side-business-reality-check 我想做副业，先帮我判断值不值得投入。
```

若未被识别，重新启动会话。这里的目录适用于本地 Claude Code，不能假定会同步到 Claude 网页、Cowork 或云会话。

### 其他 agent / 不想使用命令

- 其他支持 Agent Skills 的工具：使用上方安装提示词，让工具确认其官方技能目录；不承诺所有工具都能一键安装。
- 手动安装：点击 **Code → Download ZIP**，解压，将包含 `SKILL.md` 和 `references/` 的文件夹重命名为 `side-business-reality-check`，放入对应技能目录。
- 不支持技能的聊天工具：上传 [SKILL.md](SKILL.md)，说“请按这个文件的工作说明和我对话”。可同时上传参考文件；这是当前对话读取文档，不是永久安装。

### 怎样确认装好了？

1. 安装目录下应直接是 `SKILL.md` 和 `references/`，不能多套一层仓库文件夹。
2. `references/` 内应有 `case-lessons.md`、`hype-projects.md`、`models-and-experiments.md`、`sources.md` 四个文件。
3. 使用上面的调用方式，让 agent 确认实际读取的技能路径；仅复述仓库简介不代表安装成功。

行业实时查询需要 AI 工具具备联网功能。无联网时仍可分析个人条件，但不能冒充已经查询最新数据。

安装路径依据（核对日期：2026-10-16）：[OpenAI 官方技能文档](https://learn.chatgpt.com/docs/build-skills) · [Claude Code 官方技能文档](https://code.claude.com/docs/en/skills)。
## 复制这句话开始

> 请使用 $side-business-reality-check。我想做【你的副业想法】，目前进展是【还在想／正在调查／已经投入】。请先给我一个冷静判断，再一次问我一两个关键问题。最后建议是否值得投入，不值得时请直说，值得验证时再设计小实验。

也可以直接说：

- “我想做AI漫剧赚钱，网上说零基础就能做，帮我看看现实条件。”
- “我想做旅行账号，但还没想清楚怎么赚钱。”
- “我已经投入了钱，现在犹豫要不要继续补货。”
- “我只想增加收入，还没确定方向，先帮我梳理已有能力。”

你可以随时说“不知道”“跳过”“先总结”，不必答完整套问题，也不用提供账户、证件或详细财务信息。

## 它不会做什么

不会给你必赚项目、编造成功率或保证主业一定涨薪。不会只凭某个培训受损案例断言整个行业都是骗局，也不会以“不是绝无机会”为由鼓励你继续投入。

它来自一次线香创业复盘与实际咨询思考，并结合商业分析资料整理。案例不代表行业统计，最终判断应结合当前证据和个人处境。

## 文件

- [SKILL.md](SKILL.md)：核心说明和对话规则。
- [模型与实验](references/models-and-experiments.md)：不同生意的追问与小实验。
- [案例教训](references/case-lessons.md)：匿名化经验及表达示例。
- [副业宣传核查](references/hype-projects.md)：AI漫剧等项目的查证与判断。
- [方法来源](references/sources.md)：资料来源与实时核查边界。

欢迎通过 Issues 提交匿名化的使用反馈：哪里追问重复、哪里结论含糊、哪里需要更好的行业证据。请勿提交个人隐私、客户名单或未脱敏合同。
