# 东方题材角色 Midjourney Skill

为各类东方题材设计原创角色，并输出可直接使用的中英文 Midjourney 提示词。适用于游戏等视觉开发：从角色身份或物种出发，选择能体现题材的身体轮廓、衣装或道具，再用动作、构图和光线呈现角色。提示词保持简短，角色之间有清晰的辨识度。

## 题材范围

以下方向均可用于角色设计；其中既有故事题材，也有时代文化和视觉风格，可按具体需求组合：

- **神话与高幻想**：山海经 / 上古异兽、古风修仙 / 仙侠、东方玄幻、西游神话、封神 / 商周神话、东方海洋神话。
- **志怪与民俗**：聊斋 / 中式志怪、中式克苏鲁 / 东方诡秘、民俗恐怖、中式妖怪 / 百妖夜行、地府 / 阴曹世界、苗疆 / 巫蛊幻想、傩文化 / 原始祭祀。
- **宗教、历史与审美**：敦煌 / 飞天仙境、佛教神话 / 东方神性、道教神话 / 道法世界、古蜀 / 三星堆幻想、水墨仙境、宋韵 / 东方生活美学、盛唐幻想、东方梦境 / 诗词幻想。
- **江湖与新幻想**：武侠 / 江湖、东方废土、赛博东方 / 赛博武侠、东方蒸汽朋克、东方机关术 / 墨家幻想。

每个方向对应的角色身份与可见造型线索见 [题材与角色线索](references/theme-directions.md)。神山、鬼市、龙宫等可以辅助交代世界，但提示词仍以人物为主体。

## 适合做什么

- 从一个题材或职业出发，设计一组不同的角色，例如异兽化形者、江湖职业、志怪人物或未来机关师。
- 根据文字或图片参考提炼造型、姿态、镜头与光影，再设计原创角色。
- 修改已有角色提示词中的衣装、武器、动作或画面表现。
- 按指定数量、正反派比例、性别年龄、景别或气质生成角色系列。

## 生成方法

单条提示词通常按以下顺序组织，按角色需要取舍：

> 题材前缀 → 角色身份或物种 → 一两处关键身体特征、衣装或道具 → 一个动作 → 景别与构图 → 光线落点 → 一两个气质词 → 必要限制

角色身份或物种是起点。人形角色的衣装、道具要符合身份与题材；异兽本体或机关兽可用形体、材质和动作建立辨识度。动作、构图和光线共同突出一个视觉焦点。提示词采用一行短句，不靠人物履历、复杂配饰、特效或画质标签撑满画面。

人形角色通常使用半身或全身构图；需要展示完整轮廓的非人角色可用全身。中近景、近景在仍能看清关键造型时也可使用。背景保持简洁，把注意力留给角色。

## 输出格式

- 默认每批 5–10 组；用户指定数量优先。
- 中文和英文提示词分别放在一个代码块中，同一角色在两个代码块中的顺序一致。
- 角色名放在代码块外；代码块内每行只放一条可复制的提示词。
- 每条以题材和用途相符的前缀开头，例如“山海经题材角色设计”或“赛博东方游戏角色设计”；只有需要游戏角色时才加入“游戏”。
- 单角色画面可排除其他角色、文字和水印。古代题材且角色设定需要时才排除现代服饰；未来题材保留符合设定的科技或混合造型。

### 示例

**山海经 / 上古异兽**

```text
山海经题材异兽角色设计，鹿形异兽，额生双层黑石角，肩背覆青灰鳞甲，前足微屈回望，低机位全身侧面构图，侧光照亮角缘与鳞片，古老、戒备，无其他角色、文字、水印
```

```text
Shan Hai Jing inspired mythical beast character design, a deer-shaped beast with layered black stone horns and blue-gray scales across its shoulders and back, front legs slightly bent as it looks back, low-angle full-body side composition, sidelight on horn edges and scales, ancient and wary, no other characters, text, or watermarks
```

**聊斋 / 中式志怪**

```text
中式志怪角色设计，荒宅女画师，暗红交领衣与染墨袖口，指尖夹着未干的画笔回望，半身侧面构图，一束烛光照亮眼睛和笔尖，幽艳、镇定，无其他人物、现代服饰、文字、水印
```

```text
Chinese supernatural folklore character design, a female painter of an abandoned house in a dark red cross-collar robe with ink-stained cuffs, turning back with a wet brush between her fingers, waist-up side composition, candlelight on her eyes and the brush tip, eerie and composed, no other people, modern clothing, text, or watermarks
```

**赛博东方**

```text
赛博东方游戏角色设计，未来城巡夜剑客，黑色束袖外袍叠穿轻型机械护臂，短剑收于身侧，半身偏心构图，蓝色屏光落在护臂和侧脸，克制、警觉，无其他人物、文字、水印
```

```text
Cyber Eastern game character design, a night patrol swordsman of a future city in a black fitted-sleeve outer robe and light mechanical bracer, short sword at his side, off-center waist-up composition, blue screen light on the bracer and profile, restrained and alert, no other people, text, or watermarks
```

## 使用方式

在 Codex 中调用这个 Skill，并说明你想要的角色方向。例如：

```text
使用 $midjourney-oriental-game-characters，设计 10 个东方题材角色，覆盖山海经、聊斋、武侠和赛博东方，身份与造型不要重复。
```

```text
使用 $midjourney-oriental-game-characters，设计 6 个民俗恐怖角色，以半身构图为主，服饰和道具保持克制。
```

```text
使用 $midjourney-oriental-game-characters，参考这张图的服装层次和侧光，设计一个原创东方海洋神话角色，不复刻原角色。
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
- `references/theme-directions.md`：26 个方向的角色切入点与可见造型线索。
- `agents/openai.yaml`：Codex 中显示的 Skill 名称、说明与默认调用语。
- `README.md`：项目介绍、使用方法和输出示例。
