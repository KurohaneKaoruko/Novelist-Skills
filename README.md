# Novelist-Skills

通用小说方法论 skill 集合——不绑定任何单一项目，可挂载到任何需要写作方法论的
DSH 预设 / Agent 项目。

## 内容

**7 个方法论 skill**

| skill | 职责 |
| --- | --- |
| `novel-project` | 工程初始化与项目结构 |
| `novel-craft` | 写作工艺总纲 |
| `novel-plotting` | 情节构思 |
| `novel-prose-standards` | 行文标准 |
| `novel-ai-lexicon` | 去 AI 味词法（第二代特征） |
| `novel-continuity` | 连续性 / 设定一致性 |
| `novel-analysis` | 成稿分析 |

**6 个文风 skill（`novel-style-*`，按作品归属加载）**

`hotblood`（热血）· `lightnovel`（轻小说）· `mystery`（推理）· `romance`（言情）· `scifi`（科幻）· `xianxia`（仙侠）

## 挂载方式

skill 约定放在预设的 `skills/` 目录（`skills/<name>/SKILL.md`）。推荐以
submodule 原位挂载：

```bash
git submodule add https://github.com/KurohaneKaoruko/Novelist-Skills.git skills
```

克隆方拉取：

```bash
git clone --recurse-submodules <你的项目>
# 已克隆的项目补拉：
git submodule update --init
```

上游更新：

```bash
git submodule update --remote skills
```

## 与 DSH-Novelist 的关系

[DSH-Novelist](https://github.com/KurohaneKaoruko/DSH-Novelist)（小说助手预设）
以 submodule 形式引用本仓库，专注于 DSH 本身的适配（preset、插件、内核验证）；
本仓库保持通用，只放跨项目可复用的方法论。

## License

MIT
