# 东方题材角色 · 中英文 Midjourney 提示词 Skill

为东方题材创作原创概念角色，把题材、角色名单、造型描述或参考图整理成精炼、可复制的中英文 Midjourney 提示词。适用于角色概念探索、游戏角色视觉开发、异兽与精怪造型设计。

这是在 Codex 中使用的 Skill，输出内容是角色设计文字与提示词。生成后，将提示词复制到 Midjourney 中使用；本 Skill 本身不连接 Midjourney，也不自动出图。

## 能做什么

| 你的输入 | Skill 会完成什么 |
| --- | --- |
| 一个明确题材，例如“江南园林角色，10组” | 设计不同身份、轮廓、服装和姿态，输出对应提示词 |
| 一份角色名单 | 按原顺序展开角色，不另换选题 |
| 角色名与身体结构描述 | 保留关键设定，补充必要的动作、构图和光线 |
| 一张参考图或一组参考文字 | 提炼造型、材质、姿态或光影方法，设计原创角色 |
| 现有提示词与修改要求 | 调整指定内容，沿用其余已明确条件 |
| 尚未确定的方向 | 先选题材大组，再选具体类型；也支持混合题材和随机搭配 |

支持人形角色、兽首异人、异兽本体、机关兽、器物精怪等。非人角色以形体结构、表面材质和动作建立辨识度，不强加人脸或服装。

## 快速开始

安装后，在 Codex 聊天中使用 `$midjourney-oriental-game-characters` 加上你的需求。最简单的输入是“题材 + 数量”；无需先填完整份角色设定表。

### 1. 已有题材，直接生成

```text
使用 $midjourney-oriental-game-characters，设计10个聊斋类原创角色，参考《倩女幽魂》的幽艳气质，角色身份与造型不要重复。
```

题材已明确时直接生成，不再要求重复选择性别、职业或阵营。参考作品用于提炼视觉方法，不复刻原作的面容、标志性衣装或完整造型。

### 2. 已有角色名单，按顺序展开

```text
使用 $midjourney-oriental-game-characters。
题材：青灯妖城·夜巡异闻。
角色：掌灯狐妖、巡夜女术士、纸偶修补师、镇桥石灵、听风鸦妖、缉祟女捕快、朱印契官、忘忧茶师、雾河摆渡人、修符老匠。
每个角色一组中英文提示词。
```

也可以在每个角色后附上关键结构，例如“完整鹿首连接直立长身，巨角挂药草，双足保留蹄形”。Skill 会沿用这些结构，不把异物统一改成人形美人。

### 3. 题材未定，先选方向

```text
使用 $midjourney-oriental-game-characters，先让我选择题材，再生成10个角色。
```

先展示四大组及“混合题材”“随机搭配”；选定大组后再展示子类。明确要求随机即授权自行选型。

### 4. 使用图片参考

```text
使用 $midjourney-oriental-game-characters，参考附图的身体轮廓与服装结构，设计10个原创东方异物角色，保留我的物种方向。
```

请在当前聊天附上图片，并说明借鉴造型、动作、材质还是光影。跨聊天提及的图片需要在当前聊天重新提供。

### 5. 控制风格或修改已有结果

```text
使用 $midjourney-oriental-game-characters，沿用上一组角色，仅将姿态改为能展示装备的戒备站姿，保留服装与物种设定。
```

```text
使用 $midjourney-oriental-game-characters，设计10个东方志怪CG角色，纯米白背景，其余按角色设定选择。
```

风格由你控制，可明确指定CG、3D、2.5D、手绘、水墨或其他表现。未指定时，Skill 不主动加入风格或渲染引擎标签；需要时再添加相容的材质和渲染词。

## 默认会怎样设计

- **全身完整入镜**：人形从头顶至鞋履，非人角色保留爪足、尾部、翅翼等关键结构；坐姿或进攻姿态也保持完整。
- **镜头以平视为主**：朝向按造型展示需要选择，不套用固定四分之三视角，不使用俯视。
- **姿态服务角色**：站立展示衣装与轮廓，进攻或防御展示体态与武器，持握或操作道具展示行当特征。
- **背景单一**：默认纯色无纹理，底色按需求或配色选择，不固定黑底；不添加场景、烟雾、渐变或装饰。
- **短句表达**：每条一行，用逗号连接关键画面信息，避免人物履历、复杂场景与无关特效堆叠。
- **限制词按需添加**：不逐条重复“无场景、文字、水印”等固定尾缀。

默认每批5–10组，明确数量优先。可以补充年龄、性别倾向、正反派比例、配色、武器、道具、动作或异化程度；目标清楚时，其余细节由 Skill 补全。

## 输出是什么样

角色名称放在代码块外。中文提示词合并为一个代码块，英文合并为另一个代码块；每条一行，同一角色在两个代码块中顺序对应。

以下为单角色格式示例，风格未指定，因此不添加风格标签。

**角色：鹿首巡山灵**

中文：

```text
东方志怪角色设计，鹿首巡山灵，完整鹿首连接直立修长躯干，分叉巨角垂挂药草束，灰褐粗布披肩与蹄形双足，侧身迈步并抬手扶住药束，平视全身略侧构图，柔暖侧光照亮鹿面与草叶，古朴、警觉，纯灰无纹理背景，完整入镜
```

英文：

```text
Eastern supernatural character design, a deer-headed mountain warden, complete deer head joined to a tall upright body, branching antlers hung with herb bundles, gray-brown coarse-cloth shoulder wrap and hoof-shaped feet, stepping sideways and raising one hand to steady the herbs, eye-level full-body slight oblique view, soft warm sidelight on the deer face and leaves, rustic and vigilant, flat solid gray background without texture, entire figure in frame
```

复制中文或英文提示词到 Midjourney 使用即可；可按自己的工作习惯补充版本、画幅或其他参数。

## 支持哪些题材

题材索引覆盖26个方向，分为四组，允许按需组合：

- **神话与高幻想**：山海经 / 上古异兽、古风修仙 / 仙侠、东方玄幻、西游神话、封神 / 商周神话、东方海洋神话。
- **志怪与民俗**：聊斋 / 中式志怪、中式克苏鲁 / 东方诡秘、民俗恐怖、中式妖怪 / 百妖夜行、地府 / 阴曹世界、苗疆 / 巫蛊幻想、傩文化 / 原始祭祀。
- **宗教、历史与审美**：敦煌 / 飞天仙境、佛教神话 / 东方神性、道教神话 / 道法世界、古蜀 / 三星堆幻想、水墨仙境、宋韵 / 东方生活美学、盛唐幻想、东方梦境 / 诗词幻想。
- **江湖与新幻想**：武侠 / 江湖、东方废土、赛博东方 / 赛博武侠、东方蒸汽朋克、东方机关术 / 墨家幻想。

具体角色切入点见 [题材与角色线索](references/theme-directions.md)。美型、怪诞或恐怖程度按需求决定；美型异物的自然生长结构可参考 [美型东方异物规则与造型线索](references/elegant-supernatural-characters.md)。

## 安装与更新

需要可使用 Skills 的 Codex 环境、Git，以及本仓库的访问权限。下面以 HTTPS 安装为例：

```bash
git clone https://github.com/2053197099/midjourney-oriental-game-characters.git ~/.codex/skills/midjourney-oriental-game-characters
```

若环境设置了自定义 `CODEX_HOME`，请安装到其对应的 `skills` 目录。已配置 GitHub SSH 时，也可使用仓库的 SSH 地址。私有仓库需先配置具有访问权限的 Git 凭据。

安装后，在 Codex 的 Skill 列表确认可用，再使用 `$midjourney-oriental-game-characters` 调用。若当前会话尚未识别，重新打开会话后再检查。

更新已安装的副本：

```bash
git -C ~/.codex/skills/midjourney-oriental-game-characters pull --ff-only
```

若你修改过本地 Skill，先保存或提交自己的修改，再更新。

## 文件说明

| 文件 | 用途 |
| --- | --- |
| [SKILL.md](SKILL.md) | 角色设计流程、输出格式与自检规则 |
| [agents/openai.yaml](agents/openai.yaml) | Codex 中显示的名称、简述与默认调用语 |
| [references/theme-directions.md](references/theme-directions.md) | 26个题材方向的角色身份与可见造型线索 |
| [references/elegant-supernatural-characters.md](references/elegant-supernatural-characters.md) | 美型异物的结构、材质原则与十个造型方向 |
| README.md | 功能介绍、使用示例、安装与更新方法 |
