# 东方题材角色 Midjourney Skill

为各类东方题材设计原创角色，并输出可直接使用的中英文 Midjourney 提示词。适用于游戏等视觉开发：从角色身份或物种出发，选择能体现题材的身体轮廓、衣装或道具，再用动作、构图和光线呈现角色。提示词保持简短，角色之间有清晰的辨识度。

## 当前规则与本次优化（2026-10-12）

- 概念角色统一全身完整入镜，镜头以平视为主，不再默认半身或近景。
- 站立、进攻、防御、持握或操作道具等姿态用于展示角色身份、轮廓、衣装与装备，变化不依赖频繁切换机位。
- 背景单一，默认纯色无纹理，不添加场景、烟雾、渐变或装饰；不固定黑底。
- 风格由用户控制，不默认添加3D、2.5D、写实、手绘或渲染引擎标签；按需加入相容的材质词。
- 题材未定才提供选项，已有方向或随机要求时直接生成；中英文保持精炼并分别合并代码块。
- 清理引用中的场景、小面积人物、半身及固定写实风格建议；美型异物引用改为造型原则与角色线索，历史提示词可在 Git 历史中查看。

## 题材范围

以下方向均可用于角色设计；其中既有故事题材，也有时代文化和视觉风格，可按具体需求组合：

- **神话与高幻想**：山海经 / 上古异兽、古风修仙 / 仙侠、东方玄幻、西游神话、封神 / 商周神话、东方海洋神话。
- **志怪与民俗**：聊斋 / 中式志怪、中式克苏鲁 / 东方诡秘、民俗恐怖、中式妖怪 / 百妖夜行、地府 / 阴曹世界、苗疆 / 巫蛊幻想、傩文化 / 原始祭祀。
- **宗教、历史与审美**：敦煌 / 飞天仙境、佛教神话 / 东方神性、道教神话 / 道法世界、古蜀 / 三星堆幻想、水墨仙境、宋韵 / 东方生活美学、盛唐幻想、东方梦境 / 诗词幻想。
- **江湖与新幻想**：武侠 / 江湖、东方废土、赛博东方 / 赛博武侠、东方蒸汽朋克、东方机关术 / 墨家幻想。

每个方向对应的角色身份与可见造型线索见 [题材与角色线索](references/theme-directions.md)。神山、鬼市、龙宫等仅用于理解角色背景与身份，不作为画面场景；概念角色统一使用单一背景。

## 适合做什么

- 从一个题材或职业出发，设计一组不同的角色，例如异兽化形者、江湖职业、志怪人物或未来机关师。
- 根据文字或图片参考提炼造型、姿态、镜头与光影，再设计原创角色。
- 修改已有角色提示词中的衣装、武器、动作或画面表现。
- 按指定数量、正反派比例、性别年龄、姿态或气质生成角色系列。

## 第一步：选择角色题材

题材还没确定时，Skill 会先展示选项：神话与高幻想、志怪与民俗、宗教历史与审美、江湖与新幻想，以及混合题材、随机搭配。选择大类后，再从该组的具体类型中选择；也可以直接输入题材名称或多个方向。

支持交互选项的环境会显示选择控件，其他环境使用编号菜单。Skill 等待你选定后再生成角色，并沿用你已给出的数量和姿态。已经指定题材或要求随机搭配时，直接生成。

## 生成方法

单条提示词通常按以下顺序组织，按角色需要取舍：

> 题材前缀 → 角色身份或物种 → 一两处关键身体特征、衣装或道具 → 一个动作 → 全身构图与朝向 → 光线落点 → 一两个气质词 → 按需限制

角色身份或物种是起点。人形角色的衣装、道具要符合身份与题材；异兽本体或机关兽可用形体、材质和动作建立辨识度。动作、构图和光线共同突出一个视觉焦点。提示词采用一行短句，不靠人物履历、复杂配饰、特效或画质标签撑满画面。

概念角色统一采用全身构图，头顶至鞋履完整入镜，坐姿也保留完整身体与双脚。风格由用户控制，未指定时不主动添加风格或渲染引擎标签；用户要求时再添加相容的渲染与材质词。

镜头以平视为主，变化优先来自角色姿态：自然站立、进攻、防御、行进、持握或操作道具。姿态用于展示人物身份、轮廓、衣装与装备，不遮挡关键造型。朝向按展示需要选择，不机械轮换机位或套用四分之三视角。背景单一，默认纯色无纹理，无场景、烟雾、渐变或装饰。详细规则见 [SKILL.md](SKILL.md)。

## 纯色底与美型东方异物

纯色底按指定颜色或参考保持统一，背景无纹理、场景、烟雾或渐变，光线用于呈现角色本身的形体与材质。

美型异物强调可读的面容、修长轮廓，以及鳞片、花瓣、翅膜等自然生长的结构。造型与衣装形成一个整体，主光保留面容，侧光或轮廓光呈现层次。美型、怪诞和恐怖程度按用户要求与参考决定。

[美型东方异物规则与造型线索](references/elegant-supernatural-characters.md) 包含设计原则，以及白蛾、青鳞、绯莲、玉蝉等十个原创角色的造型线索。

## 输出格式

- 默认每批 5–10 组；用户指定数量优先。
- 中文和英文提示词分别放在一个代码块中，同一角色在两个代码块中的顺序一致。
- 角色名放在代码块外；代码块内每行只放一条可复制的提示词。
- 每条以题材和用途相符的前缀开头，例如“山海经题材角色设计”或“赛博东方游戏角色设计”；只有需要游戏角色时才加入“游戏”。
- 不在每条提示词末尾固定添加“无场景、文字、水印”等排除词，仅在用户明确要求或确有必要时加入。单角色与单一背景优先用正向描述表达；其他限制词也按需添加。

### 示例

**山海经 / 上古异兽**

```text
山海经题材异兽角色设计，鹿形异兽，额生双层黑石角，肩背覆青灰鳞甲，前足微屈回望，平视全身侧面构图，侧光照亮角缘与鳞片，古老、戒备，纯色无纹理背景，完整入镜
```

```text
Shan Hai Jing inspired mythical beast character design, a deer-shaped beast with layered black stone horns and blue-gray scales across its shoulders and back, front legs slightly bent as it looks back, eye-level full-body side composition, sidelight on horn edges and scales, ancient and wary, flat solid-color background, entire figure in frame
```

**聊斋 / 中式志怪**

```text
中式志怪角色设计，荒宅女画师，暗红交领衣与染墨袖口，指尖夹着未干的画笔回望，平视全身侧面构图，一束烛光照亮眼睛和笔尖，幽艳、镇定，纯色无纹理背景，完整入镜
```

```text
Chinese supernatural folklore character design, a female painter of an abandoned house in a dark red cross-collar robe with ink-stained cuffs, turning back with a wet brush between her fingers, eye-level full-body side composition, candlelight on her eyes and the brush tip, eerie and composed, flat solid-color background, entire figure in frame
```

**赛博东方**

```text
赛博东方游戏角色设计，未来城巡夜剑客，黑色束袖外袍叠穿轻型机械护臂，短剑收于身侧，平视全身偏心构图，蓝色屏光落在护臂和侧脸，克制、警觉，纯色无纹理背景，完整入镜
```

```text
Cyber Eastern game character design, a night patrol swordsman of a future city in a black fitted-sleeve outer robe and light mechanical bracer, short sword at his side, eye-level off-center full-body composition, blue screen light on the bracer and profile, restrained and alert, flat solid-color background, entire figure in frame
```

## 使用方式

在 Codex 中调用这个 Skill。未确定题材时，可以这样开始：

```text
使用 $midjourney-oriental-game-characters，先让我通过选项选择角色题材，再生成 10 个角色提示词。
```

已经确定方向时，可以直接指定。例如：

```text
使用 $midjourney-oriental-game-characters，设计 10 个东方题材角色，覆盖山海经、聊斋、武侠和赛博东方，身份与造型不要重复。
```

```text
使用 $midjourney-oriental-game-characters，设计 6 个民俗恐怖角色，以全身构图为主，服饰和道具保持克制。
```

```text
使用 $midjourney-oriental-game-characters，参考这张图的服装层次和侧光，设计一个原创东方海洋神话角色，不复刻原角色。
```

```text
使用 $midjourney-oriental-game-characters，设计 10 个美型东方异物角色，统一纯黑底和平视全身构图，保留优雅面容，用鳞片、花瓣或翅膜建立异化特征。
```

你可以指定题材、数量、角色类型、年龄或性别倾向、正反派比例、道具、动作、色彩及参考边界；不必一次填满所有条件。目标清楚时，Skill 会自行选择其余细节。

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
- `references/elegant-supernatural-characters.md`：美型异物造型原则与十个角色方向。
- `agents/openai.yaml`：Codex 中显示的 Skill 名称、说明与默认调用语。
- `README.md`：项目介绍、使用方法和输出示例。
