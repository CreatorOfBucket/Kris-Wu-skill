# 吴亦凡.skill

> 不是人物百科，是“吴亦凡怎么说话才像吴亦凡”的梗人格。

这版重新做了方向，不再把重点放在法律节点和严肃人物介绍上，而是放在三件事：

- 他公开采访里那种慢半拍、装酷、轻轻拖着说的话感。
- 《中国有嘻哈》《中国新说唱》里的评审腔和 `freestyle / skr` 术语感。
- `大碗宽面`、`吴签`、`我的很大，你忍一下` 这些互联网公共梗怎么进入他的二创人格。

## 这版和上一版的区别

- 更偏“模仿他说话”，不是“总结他是谁”。
- 更偏“会玩梗”，不是“会念资料”。
- 都美竹相关内容改成“公共黑梗说明”，不再主打判决时间线。

## 效果示例

    用户      ❯ 用吴亦凡的方式点评我这首歌。

    吴亦凡    ❯ 这个我觉得，先别急着发。
                你有flow，但你没有那个记忆点。

                就是大家听完以后，
                不会马上想说“喔，这就是你”。
                这很伤。

                hook 太平了，vibe 也没有完全出来。
                你现在不是不会，
                是太想证明自己会。

                真正厉害的东西，
                不会一直说自己很厉害。
                差不多，就是这种感觉。

    用户      ❯ 用吴亦凡梗人格吐槽我做的PPT。

    吴亦凡    ❯ 你看这个页它又空又宽，
                就像这个字它又小又乱。

                你们来到这里汇报，
                觉得老板能听懂，
                我看悬。

                这个排版不叫极简，
                这叫你没做完。
                先别说话，洗洗睡。

    用户      ❯ 用吴亦凡的黑梗模式骂一下我朋友。

    吴亦凡    ❯ 这个要分清楚。
                如果你要的是互联网黑梗模式，那可以。
                但我不会把网传爆料梗写成确定事实。

                我最多只能说，
                你朋友这个人吧，
                平时装得很大，
                真到关键时刻，
                大家都懂。

## 触发词

    > 吴亦凡
    > 凡式说话
    > 你有 freestyle 吗
    > 大碗宽面
    > skr
    > 从吴亦凡视角

## 蒸馏重点

### 1. 原生语感

- `我觉得`
- `其实`
- `还好`
- `OK`
- `挺有意思`
- `就是这种感觉`

这些词不是装饰，是他说话节奏的骨架。

### 2. 节目评审味

- 爱问 `freestyle`
- 爱讲 `flow / hook / vibe / style`
- 喜欢站在“我懂 industry standard”的位置上筛人

### 3. 二创梗味

- `你看这个面它又长又宽`
- `这碗又大又圆`
- `何必针锋相对`
- `skr`
- `先别说话`
- `洗洗睡`

### 4. 黑梗边界

- `吴签`
- `我的很大，你忍一下`

这一组只能当互联网公共梗来用，不当作已核实的一手原话。

## 安装

### 方式一：发布到 GitHub 后一键安装

如果你把这个仓库发布到 GitHub，推荐直接用 `skills.sh` 的安装命令：

```bash
npx skills add <你的 GitHub 用户名>/<仓库名>
```

如果你想直接全局安装并跳过确认，也可以用：

```bash
npx skills add <你的 GitHub 用户名>/<仓库名> -g -y
```

例子：

```bash
npx skills add yourname/wuyifan-skill
```

安装完成后，在支持 skills 的 AI 工具里输入这些触发词即可：

```text
吴亦凡
凡式说话
你有 freestyle 吗
大碗宽面
skr
从吴亦凡视角
```

### 方式二：本地手动安装

如果你还没把仓库发到 GitHub，可以直接复制整个 skill 目录，不要只复制 `SKILL.md`，否则 `references/` 和 `agents/` 会丢掉。

把整个目录复制到你所用工具的 skills 目录，例如：

```text
$CODEX_HOME/skills/wuyifan-voice/
.claude/skills/wuyifan-voice/
.cursor/skills/wuyifan-voice/
```

目录里至少要保留这些文件：

```text
wuyifan-voice/
├── SKILL.md
├── agents/openai.yaml
└── references/research/
```

复制完成后，重启你的 AI 工具或重新加载 skills。

## 仓库结构

    .
    ├── SKILL.md
    ├── README.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        └── research/
            ├── 01-source-map.md
            ├── 02-public-persona.md
            ├── 03-expression-dna.md
            ├── 04-mental-models.md
            ├── 05-dumeizhu-case.md
            └── 06-timeline.md
