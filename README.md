# 东方游戏角色 Midjourney Skill

为东方武侠、仙侠、历史奇幻与神话游戏设计原创角色，并输出可直接使用的中英文 Midjourney 提示词。这个 Skill 聚焦人物的身份、衣装、道具、动作、构图和光线，让一组角色各有辨识度，同时保持提示词简短。

## 适合做什么

- 从一个题材或职业出发，设计一组不同的游戏角色，例如武侠门派人物、江湖职业或仙侠修行者。
- 根据文字或图片参考提炼造型、姿态、镜头与光影，再设计原创角色。
- 修改已有角色提示词中的衣装、武器、动作或画面表现。
- 按指定数量、正反派比例、性别年龄、景别或气质生成角色系列。

本项目处理**角色提示词**。纯场景、建筑和环境叙事可使用对应的场景 Skill；本项目不直接调用 Midjourney 生成图片。

## 生成方法

单条提示词通常按以下顺序组织，按角色需要取舍：

> 题材前缀 → 角色身份 → 一两处衣装特征与必要道具 → 一个动作 → 景别与构图 → 光线落点 → 一两个气质词 → 必要限制

角色身份是起点。衣装和道具要符合职业与题材；动作、构图和光线共同突出一个视觉焦点。提示词采用一行短句，不靠人物履历、复杂配饰、特效或画质标签撑满画面。

通常使用半身或全身构图。中近景、近景在仍能看清衣装或关键道具，并有助于突出角色时也可使用。背景保持简洁，把注意力留给人物。

## 输出格式

- 默认每批 5–10 组；用户指定数量优先。
- 中文和英文提示词分别放在一个代码块中，同一角色在两个代码块中的顺序一致。
- 角色名放在代码块外；代码块内每行只放一条可复制的提示词。
- 每条以题材前缀开头，例如“东方武侠游戏角色设计”或“东方仙侠游戏角色设计”。
- 单人古风角色默认排除其他人物、现代服饰、文字和水印；用户另有要求时调整。

### 示例

**武侠**

```text
东方武侠游戏角色设计，边关女巡哨，灰褐窄袖短袄与皮革护肩，单手扶短弓回望，半身偏心构图，夕光落在弓背和侧脸，沉着、敏锐，无其他人物、现代服饰、文字、水印
```

```text
Eastern wuxia game character design, a female frontier scout in a gray-brown narrow-sleeved jacket and leather shoulder guard, one hand on a short bow as she looks back, off-center waist-up composition, sunset light on the bow and her profile, composed and alert, no other people, modern clothing, text, or watermarks
```

**仙侠**

```text
东方仙侠游戏角色设计，守炉青年丹师，青灰束袖道袍与暗铜护腕，手托一枚新成丹药，半身侧面构图，炉火暖光照亮掌心和衣袖，谨慎、专注，无其他人物、现代服饰、文字、水印
```

```text
Eastern xianxia game character design, a young furnace alchemist in a blue-gray fitted-sleeve robe and dark copper bracers, holding a freshly made pill, waist-up side composition, warm furnace light on the palm and sleeve, careful and focused, no other people, modern clothing, text, or watermarks
```

## 使用方式

在 Codex 中调用这个 Skill，并说明你想要的角色方向。例如：

```text
使用 $midjourney-oriental-game-characters，设计 10 个东方武侠角色，正派和反派各 5 个，职业与造型不要重复。
```

```text
使用 $midjourney-oriental-game-characters，设计 6 个仙侠门派角色，以半身构图为主，衣装和法器保持简洁。
```

```text
使用 $midjourney-oriental-game-characters，参考这张图的服装层次和侧光，设计一个原创江湖角色，不复刻原角色。
```

你可以指定题材、数量、角色类型、年龄或性别倾向、正反派比例、道具、动作、景别、色彩及参考边界；不必一次填满所有条件。目标清楚时，Skill 会自行选择其余细节。

## 参考与原创

图片参考用于提炼轮廓、服装结构、材质、姿态和光线；成组提示词可用于提炼信息顺序和句式密度。参考作品中的标志性面容、服装、武器组合及完整造型不会被直接复刻。用户只要求修改某一项时，仅调整相关内容。

## 安装

本仓库根目录就是 Codex Skill。获得仓库访问权限并配置 GitHub SSH 后，可在另一台电脑上安装：

```bash
git clone git@github.com:2053197099/midjourney-oriental-game-characters.git ~/.codex/skills/midjourney-oriental-game-characters
```

若设置了自定义 `CODEX_HOME`，请将仓库放在对应的 `skills` 目录。安装后在 Codex 中使用 `$midjourney-oriental-game-characters` 调用。

## 仓库文件

- `SKILL.md`：实际执行的角色设计与提示词规则。
- `agents/openai.yaml`：Codex 中显示的 Skill 名称、说明与默认调用语。
- `README.md`：项目介绍、使用方法和输出示例。
