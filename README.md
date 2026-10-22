# IIIA - AI 参与指数

![IIIA-3*](https://img.shields.io/badge/IIIA-3*-A865B3)

“AI 参与指数”（Indice d'implication de l'intelligence artificielle，IIIA）尝试提出一套区分作品中 AI 参与度的详细档位分类建议，旨在帮助创作者、受众以及相关行业人员清晰地界定和理解一件作品在构思与制作过程中 AI 参与的程度。

IIIA 的判定依据是“这件作品是如何被想出来、又是如何被做出来的”，与其发布平台、篇幅、商业属性无关。

## 适用范围

IIIA 起源于对视频的界定，如今努力适用于一切可被观看、阅读、聆听或使用的作品：视频、音频、文字、图像与设计、音乐、代码等。

IIIA 中所说的 AI，均指能够输出大规模、有规律结果的生成式 AI（这类模型近年的普及引发了广泛的社会讨论）。对于更多领域的 AI，如传统机器学习算法、AlphaGo、游戏中基于行为树或状态机的 NPC 等，均不在 IIIA 的考虑范围。

IIIA 不评价作品好坏，只描述 AI 的参与程度。

IIIA 只判定最终呈现的作品，不嵌套判定作品背后的工具或呈现技术。例如，使用 AI 开发出一款剪辑软件，再由人类操作该软件手动剪辑视频，则该视频**不会**因使用了该剪辑软件而被判定为使用 AI。

IIIA 是一份建议性质的尝试，而非任何强制或非强制的标准，没有认证机构。是否采用、如何采用 IIIA，由创作者自愿决定。（当然大家如果认同的话我会很开心就是了。）

## 两个判定维度和一个修正选项

一个作品的 IIIA 档位由两个维度 + 一个修正选项判定而成。

### 判定维度

- **主旨思路**：缩写为 Z（代表 zhǔzhǐ），主要用于区分“由谁来决定这件作品想表达什么、怎么组织”，覆盖作品的立意、观点、叙事结构、逻辑链、脚本、创意方向等。
- **实现过程**：缩写为 S（代表 shíxiàn），主要用于区分“这件作品由谁制作完成”，覆盖作品的素材生成、撰写与润色、编排、剪辑、后期、混音、渲染等。

两个维度各自独立判档，互不折算。

### 修正选项

考虑到谈论 AI 本身的作品可能更多或更少地使用 AI 创作，因此引入“作品主题是否围绕 AI”作为修正选项。修正选项不改变作品的 IIIA 档位判定，目的是为比较不同作品的 IIIA 提供更多参考。

## 如何判定 IIIA

确定 IIIA 的过程可概括为以下步骤：

- 确定 Z 和 S 档位；
- 确定 IIIA 的表示。

### 确定 Z 和 S 档位

其中，Z 和 S 档位用 0～5 的整数表示，依照以下两表决定。

#### 主旨思路（Z）

| Z | 判定标准 |
| - | -------- |
| 0 | 作品完全由人类完成。立意、观点、叙事与逻辑链均由人工构思，AI 未参与。 |
| 1 | 作品完全由人类完成，AI 仅作为工具启发灵感或提供参考（如头脑风暴关键词、热点分析），不直接生成观点。 |
| 2 | 作品主要由人类完成，AI 进行基础辅助工作（如语法检查、简单文本润色、事实核对提示）。 |
| 3 | AI 完成大量内容模块（如分镜脚本、观点论据、脚本初稿），但经人工深度修改、审核、核实事实并最终定稿，人类保留关键决策权。 |
| 4 | AI 主导内容生产的完整逻辑链（如评论的论点推演、故事线设计），人工仅进行有限润色或局部调整（如修改不当表述）。 |
| 5 | AI 独立产出完整内容，无人工干预创作过程。 |

#### 实现过程（S）

| S | 判定标准 |
| - | -------- |
| 0 | 作品完全由人类完成。所有素材均为人工创作或实拍，剪辑、排版、后期完全手动，AI 未参与。 |
| 1 | 作品完全由人类完成，AI 仅作为工具提供辅助性灵感（如图片搜索建议、音乐片段推荐）。 |
| 2 | 作品主要由人类完成，AI 局部生成少量素材（如背景图、虚拟场景），人工完成素材整合与核心制作。 |
| 3 | AI 完成部分关键素材（如主要配图、背景音乐、部分片段），但所有素材均经人工严格筛选、编辑或整合。 |
| 4 | AI 主导创作，生成大部分或全部素材，人工仅进行抽查式审核。 |
| 5 | AI 全流程自主完成所有素材的生成、选择、编辑与合成。人类无任何创作干预，仅执行操作（如上传、发布）。 |

### 确定 IIIA 的表示

IIIA 的表示由数字部分和修正符号组成。

#### 数字表示

确定 Z 和 S 档位后，依照下表确定数字表示：

| 条件 | 标注形式 | 示例 |
| ---- | -------- | ---- |
| \|Z - S\| ≤ 1 | 取两者中较大值，写作**一位数字** | Z=2，S=3 → 表示为`3` |
| \|Z - S\| ≥ 2 | 按“**Z 在前、S 在后**”连续写作**两位数字** | Z=0，S=4 → 表示为`04` |

#### 修正符号

若作品本身以 AI 为主题，则在数字表示末尾添加星形符号。星形符号可以是任意“肉眼看起来可以识别为星星”的字符或图片，推荐采用星号（`*`）。若作品本身不以 AI 为主题，则不添加任何额外符号。

#### 注意事项

- 作品的 IIIA 数字部分请勿删除先导 0，如`03`和`3`被视作不同的 IIIA 档位。
- \|Z - S\| ≤ 1 时 IIIA 的档位为单数字，这一模糊度是有意保留的。也就是说，IIIA 不存在形如`23`的档位，应直接判定为`3`。
- 是否添加修正符号的唯一判断依据是作品讨论的主题。

### 判定示例

以下是一些场景下作品的 IIIA 示例，供参考。

| 类型   | 作品情形                                                     | Z    | S    | IIIA  |
| ------ | ------------------------------------------------------------ | ---- | ---- | ----- |
| 视频   | 全程手写手拍，未用任何 AI 功能；主题是数码产品               | 0    | 0    | `0`   |
| 视频   | AI 生成全部素材与剪辑，但选题、叙事结构与最终结论由人工定调并审核，人工只抽查了两处明显错误；主题是短剧  | 3    | 4    | `4`   |
| 文字   | 人类从头撰写全文，用 AI 做了一轮语法校对与润色；主题是公众号的广告 | 0    | 2    | `02`  |
| 文字   | AI 生成段落，人工重写结构与论据并逐条核实事实；主题是爱情小说 | 3    | 2    | `3`   |
| 图像   | 人类在 AI 展览拍摄打卡照片，用修图软件自带的磨皮功能处理后出图，并未输入提示词 | 0    | 0    | `0*`  |
| 设计   | AI 生成主视觉，人类定方案与版式并精修                        | 1    | 3    | `13`  |
| 音乐   | 人类作曲与编曲，AI 生成部分音色与伴奏轨                      | 1    | 3    | `13`  |
| 音乐   | AI 生成旋律及歌词，人类完成编曲、混音与母带                  | 4    | 2    | `42`  |
| 代码   | 人类设计架构与接口，AI 补全实现，人工逐段审核；项目目的是接入某大模型 API | 1    | 3    | `13*` |
| 代码   | AI 生成核心算法，人类补测试与边界处理；项目是手游            | 4    | 2    | `42`  |
| 多媒介 | AI 生成全部内容，人类只负责点击上传；主题讲述 AI 伦理        | 5    | 5    | `5*`  |

## 如何展示 IIIA

创作者在发布作品时，可根据实际制作情况参考本分类建议标注 AI 参与档位。

标注有三种方式，可按场合任选：

- 以文本形式标注；
- 以徽章形式标注；
- 以贴纸形式标注。

推荐将 IIIA 标注于作品靠近开头的位置，方便受众及时了解相关情况。如果可能，请在标注时附带 IIIA 的说明网址（`https://ersansan233.github.io/IIIA/`），方便更多人了解 IIIA。

### 以文本形式标注

可在作品中以如下形式的文字展示作品的 IIIA：

- IIIA13；
- `AI参与指数：3`；
- 本作品 IIIA：`0*`。

推荐采用“IIIA 前缀+连写 IIIA 档位”的形式，如“IIIA24”。

### 以徽章形式标注

IIIA 支持 Shields.io 网站徽章。如果项目带有 README.md，或其他可以解析徽章网址的文件，可以使用徽章来展示 IIIA。

可以使用拼接模板制作自己的 IIIA 徽章，也可以从下方表格中选取。

#### 拼接模板

```
https://img.shields.io/badge/IIIA-<档位>[*]-<颜色>
```

- `<档位>`：按上文规则得出的单数字（如 `3`）或两位数（如 `24`）。
- `[*]`：作品以 AI 为主题时加星号，否则省略。
- `<颜色>`：取 Z 与 S 中的**较大值**所对应的颜色，使其反映该作品 AI 参与的最高程度。

| 较大位 | 0 | 1 | 2 | 3 | 4 | 5 |
| ------ | - | - | - | - | - | - |
| 颜色代码 | `FAB689` | `D9A295` | `B97CAC` | `A865B3` | `9370DB` | `4D6BFE` |

#### 不含修正符号的 IIIA 档位

| Z \ S | 0 | 1 | 2 | 3 | 4 | 5 |
| ------ | - | - | - | - | - | - |
| **0** | [![IIIA-0](https://img.shields.io/badge/IIIA-0-FAB689)](https://github.com/ErSanSan233/IIIA) | [![IIIA-1](https://img.shields.io/badge/IIIA-1-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-02](https://img.shields.io/badge/IIIA-02-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-03](https://img.shields.io/badge/IIIA-03-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-04](https://img.shields.io/badge/IIIA-04-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-05](https://img.shields.io/badge/IIIA-05-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **1** | [![IIIA-1](https://img.shields.io/badge/IIIA-1-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-1](https://img.shields.io/badge/IIIA-1-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2](https://img.shields.io/badge/IIIA-2-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-13](https://img.shields.io/badge/IIIA-13-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-14](https://img.shields.io/badge/IIIA-14-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-15](https://img.shields.io/badge/IIIA-15-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **2** | [![IIIA-20](https://img.shields.io/badge/IIIA-20-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2](https://img.shields.io/badge/IIIA-2-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2](https://img.shields.io/badge/IIIA-2-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3](https://img.shields.io/badge/IIIA-3-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-24](https://img.shields.io/badge/IIIA-24-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-25](https://img.shields.io/badge/IIIA-25-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **3** | [![IIIA-30](https://img.shields.io/badge/IIIA-30-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-31](https://img.shields.io/badge/IIIA-31-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3](https://img.shields.io/badge/IIIA-3-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3](https://img.shields.io/badge/IIIA-3-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4](https://img.shields.io/badge/IIIA-4-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-35](https://img.shields.io/badge/IIIA-35-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **4** | [![IIIA-40](https://img.shields.io/badge/IIIA-40-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-41](https://img.shields.io/badge/IIIA-41-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-42](https://img.shields.io/badge/IIIA-42-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4](https://img.shields.io/badge/IIIA-4-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4](https://img.shields.io/badge/IIIA-4-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5](https://img.shields.io/badge/IIIA-5-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **5** | [![IIIA-50](https://img.shields.io/badge/IIIA-50-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-51](https://img.shields.io/badge/IIIA-51-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-52](https://img.shields.io/badge/IIIA-52-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-53](https://img.shields.io/badge/IIIA-53-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5](https://img.shields.io/badge/IIIA-5-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5](https://img.shields.io/badge/IIIA-5-4D6BFE)](https://github.com/ErSanSan233/IIIA) |

#### 含修正符号的 IIIA 档位

| Z \ S | 0 | 1 | 2 | 3 | 4 | 5 |
| ------ | - | - | - | - | - | - |
| **0** | [![IIIA-0*](https://img.shields.io/badge/IIIA-0*-FAB689)](https://github.com/ErSanSan233/IIIA) | [![IIIA-1*](https://img.shields.io/badge/IIIA-1*-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-02*](https://img.shields.io/badge/IIIA-02*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-03*](https://img.shields.io/badge/IIIA-03*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-04*](https://img.shields.io/badge/IIIA-04*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-05*](https://img.shields.io/badge/IIIA-05*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **1** | [![IIIA-1*](https://img.shields.io/badge/IIIA-1*-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-1*](https://img.shields.io/badge/IIIA-1*-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2*](https://img.shields.io/badge/IIIA-2*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-13*](https://img.shields.io/badge/IIIA-13*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-14*](https://img.shields.io/badge/IIIA-14*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-15*](https://img.shields.io/badge/IIIA-15*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **2** | [![IIIA-20*](https://img.shields.io/badge/IIIA-20*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2*](https://img.shields.io/badge/IIIA-2*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2*](https://img.shields.io/badge/IIIA-2*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3*](https://img.shields.io/badge/IIIA-3*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-24*](https://img.shields.io/badge/IIIA-24*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-25*](https://img.shields.io/badge/IIIA-25*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **3** | [![IIIA-30*](https://img.shields.io/badge/IIIA-30*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-31*](https://img.shields.io/badge/IIIA-31*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3*](https://img.shields.io/badge/IIIA-3*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3*](https://img.shields.io/badge/IIIA-3*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4*](https://img.shields.io/badge/IIIA-4*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-35*](https://img.shields.io/badge/IIIA-35*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **4** | [![IIIA-40*](https://img.shields.io/badge/IIIA-40*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-41*](https://img.shields.io/badge/IIIA-41*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-42*](https://img.shields.io/badge/IIIA-42*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4*](https://img.shields.io/badge/IIIA-4*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4*](https://img.shields.io/badge/IIIA-4*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5*](https://img.shields.io/badge/IIIA-5*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **5** | [![IIIA-50*](https://img.shields.io/badge/IIIA-50*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-51*](https://img.shields.io/badge/IIIA-51*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-52*](https://img.shields.io/badge/IIIA-52*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-53*](https://img.shields.io/badge/IIIA-53*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5*](https://img.shields.io/badge/IIIA-5*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5*](https://img.shields.io/badge/IIIA-5*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |

### 以贴纸形式标注

可以将 IIIA 做成任何形式的图片，展示在作品的任何位置。以图片形式展示的 IIIA 称作 IIIA 贴纸。

本项目带有贴纸制作器（`/docs/sticker.html`），方便制作各档位 IIIA 贴纸。

## 贡献

如果您认为本档位分类建议存在不完善的地方，或者有更好的建议，欢迎通过提交 issue 或 pull request 的方式参与贡献。

## 版本

当前版本 1.1。更新日志见 [CHANGELOG.md](CHANGELOG.md)，1.0 版本存档见 [versions/v1.md](versions/v1.md)。

IIIA 目前还能坚持向下兼容。

## 许可

本档位分类建议库采用 MIT 许可，您可以在遵循许可协议的前提下自由使用和传播。
