# IIIA - AI参与指数

![IIIA-3*](https://img.shields.io/badge/IIIA-3*-A865B3)

“AI参与指数”（Indice d'implication de l'intelligence artificielle，IIIA）尝试提出一套区分作品中AI参与度的详细等级标准，旨在帮助创作者、受众以及相关行业人员清晰地界定和理解一件作品在构思与制作过程中AI参与的程度。

> 当前版本 **1.1**（尚未发布）。改进日志见 [CHANGELOG.md](CHANGELOG.md)，1.0 版本存档见 [versions/v1.md](versions/v1.md)。

---

## 适用范围

IIIA 适用于一切可被观看、阅读、聆听或使用的作品：视频、音频与播客、文字、图像与设计、音乐、代码等。判定对象始终是“这件作品是如何被想出来、又是如何被做出来的”，与其发布平台、篇幅、商业属性无关。

对于不含声音或画面的作品，按其在自身媒介中对应的环节判定即可。例如文字作品的“实现过程”包含文字生成、润色、排版、配图；音乐作品的“实现过程”包含编曲、音色生成、混音与母带。

---

## 两个维度

| 维度 | 缩写 | 回答的问题 | 覆盖环节 |
| ---- | ---- | ---------- | -------- |
| **主旨思路** | Z（zhǔzhǐ） | 这件作品“想表达什么、怎么组织”由谁完成 | 立意、观点、叙事结构、逻辑链、脚本、创意方向 |
| **实现过程** | S（shíxiàn） | 这件作品“怎么被做出来”由谁完成 | 素材生成、撰写与润色、编排、剪辑、后期、混音、渲染 |

两个维度各自独立打分，互不折算。同一件作品完全可能出现“人类想、AI 做”或“AI 想、人类做”的交叉情形，这正是双维度存在的意义。

---

## 维度判定表

### 主旨思路（Z）

| Z | 判定标准 |
| - | -------- |
| 0 | 完全由人类完成。立意、观点、叙事与逻辑链均由人工构思，AI 未参与。 |
| 1 | 完全由人类完成，AI 仅作为工具启发灵感或提供参考（如头脑风暴关键词、热点分析），不直接生成观点。 |
| 2 | 主要由人类完成，AI 进行基础辅助工作（如语法检查、简单文本润色、事实核对提示）。 |
| 3 | AI 完成大量内容模块（如分镜脚本、观点论据、脚本初稿），但经人工深度修改、审核、核实事实并最终定稿，人类保留关键决策权。 |
| 4 | AI 主导内容生产的完整逻辑链（如评论的论点推演、故事线设计），人工仅进行有限润色或局部调整（如修改不当表述）。 |
| 5 | AI 独立产出完整内容，无人工干预创作过程。 |

### 实现过程（S）

| S | 判定标准 |
| - | -------- |
| 0 | 完全由人类完成。所有素材均为人工创作或实拍，剪辑、排版、后期完全手动，AI 未参与。 |
| 1 | 完全由人类完成，AI 仅作为工具提供辅助性灵感（如图片搜索建议、音乐片段推荐）。 |
| 2 | 主要由人类完成，AI 局部生成少量素材（如背景图、虚拟场景），人工完成素材整合与核心制作。 |
| 3 | AI 完成部分关键素材（如主要配图、背景音乐、部分片段），但所有素材均经人工严格筛选、编辑或整合。 |
| 4 | AI 主导创作，生成大部分或全部素材，人工仅进行抽查式审核。 |
| 5 | AI 全流程自主完成所有素材的生成、选择、编辑与合成。人类无任何创作干预，仅执行操作（如上传、发布）。 |

---

## 合成规则

设主旨思路得分为 Z，实现过程得分为 S：

| 条件 | 标注形式 | 示例 |
| ---- | -------- | ---- |
| \|Z − S\| ≤ 1 | 取两者中较大值，写作**单数字** | Z2 S3 → `IIIA3` |
| \|Z − S\| ≥ 2 | 按“**主旨位在前、实现位在后**”写作**两位数** | Z2 S4 → `IIIA24` |

- 两位数中第一位是主旨思路、第二位是实现过程，先导零保留，如 `IIIA05` 表示主旨 0、实现 5。
- 差值 ≤ 1 时折叠为单数字，意味着 `IIIA3` 可能对应 Z/S 为 3-3、3-2 或 2-3 三种情形。这一模糊度是有意保留的。
- 全部两位数等级共 20 种：`IIIA02` `IIIA03` `IIIA04` `IIIA05` · `IIIA13` `IIIA14` `IIIA15` · `IIIA20` `IIIA24` `IIIA25` · `IIIA30` `IIIA31` `IIIA35` · `IIIA40` `IIIA41` `IIIA42` · `IIIA50` `IIIA51` `IIIA52` `IIIA53`

### 星号（\*）

修正选项。**作品本身以 AI 为主题时，在其等级后加星号**，如 `IIIA2*`、`IIIA24*`。判断依据是作品讨论的对象，与其制作方式无关。

---

## 示例

| 类型 | 作品情形 | Z | S | 标注 |
| ---- | -------- | - | - | ---- |
| 视频 | 全程手写手拍，未用任何 AI 功能 | 0 | 0 | `IIIA0` |
| 视频 | AI 写完整剧本且几乎未改，自己实拍、自己配音、用人类创作的音乐 | 4 | 0 | `IIIA40` |
| 视频 | AI 生成全部素材与剪辑，人工只抽查了两处明显错误 | 3 | 4 | `IIIA4` |
| 播客 | 人类定选题与全部观点，AI 完成撰稿、语音合成、配乐与剪辑 | 0 | 5 | `IIIA05` |
| 文字 | 人类撰写全文，用 AI 做了一轮语法校对与润色 | 0 | 2 | `IIIA02` |
| 文字 | AI 生成初稿，人工重写结构与论据并逐条核实事实 | 3 | 2 | `IIIA3` |
| 图像 | 人类完成拍摄，用 AI 修图（磨皮、替换背景）后出图 | 0 | 3 | `IIIA03` |
| 设计 | 人类定方案与版式，AI 生成主视觉并经人工精修 | 1 | 3 | `IIIA13` |
| 音乐 | 人类作曲与编曲，AI 生成部分音色与伴奏轨 | 1 | 3 | `IIIA13` |
| 音乐 | AI 生成旋律，人类完成编曲、混音与母带 | 4 | 2 | `IIIA42` |
| 代码 | 人类设计架构与接口，AI 补全实现，人工逐段 review | 1 | 3 | `IIIA13` |
| 代码 | AI 生成核心算法，人类补测试与边界处理 | 4 | 2 | `IIIA42` |
| 多媒介 | AI 生成全部内容，人类只点上传；主题讲述 AI 伦理 | 5 | 5 | `IIIA5*` |

---

## 使用说明

创作者在发布作品时，可根据实际制作情况参考本标准标注 AI 参与等级，以“AI参与指数：`等级`”或“IIIA: `等级`”字样标注，或展示相应等级[贴纸](贴纸)，让受众更清晰地了解作品的创作过程。

- `AI参与指数：2` —— 人类主导，两个维度的 AI 参与程度接近 2。
- `IIIA: 24*` —— 主旨思路 2、实现过程 4，作品主题围绕 AI。

> **关于贴纸**：现有贴纸仅覆盖单数字等级（含带星版本共 12 张），两位数等级的贴纸方案尚未确定。

---

## 徽章

如果您的项目带有 README.md 文件，可以使用如下徽章来展示您项目的 IIIA。

### 拼接模板

```
https://img.shields.io/badge/IIIA-<等级>[*]-<颜色>
```

- `<等级>`：按合成规则得出的单数字（如 `3`）或两位数（如 `24`）。
- `[*]`：作品以 AI 为主题时加星号，否则省略。
- `<颜色>`：取 Z 与 S 中的**较大值**所对应的颜色，使其反映该作品 AI 参与的最高程度。

| 较大位 | 0 | 1 | 2 | 3 | 4 | 5 |
| ------ | - | - | - | - | - | - |
| 颜色代码 | `FAB689` | `D9A295` | `B97CAC` | `A865B3` | `9370DB` | `4D6BFE` |

### 全部等级（不带星号）

行为主旨思路 Z，列为实现过程 S，共 36 种：

| Z ＼ S | 0 | 1 | 2 | 3 | 4 | 5 |
| ------ | - | - | - | - | - | - |
| **0** | [![IIIA-0](https://img.shields.io/badge/IIIA-0-FAB689)](https://github.com/ErSanSan233/IIIA) | [![IIIA-1](https://img.shields.io/badge/IIIA-1-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-02](https://img.shields.io/badge/IIIA-02-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-03](https://img.shields.io/badge/IIIA-03-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-04](https://img.shields.io/badge/IIIA-04-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-05](https://img.shields.io/badge/IIIA-05-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **1** | [![IIIA-1](https://img.shields.io/badge/IIIA-1-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-1](https://img.shields.io/badge/IIIA-1-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2](https://img.shields.io/badge/IIIA-2-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-13](https://img.shields.io/badge/IIIA-13-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-14](https://img.shields.io/badge/IIIA-14-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-15](https://img.shields.io/badge/IIIA-15-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **2** | [![IIIA-20](https://img.shields.io/badge/IIIA-20-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2](https://img.shields.io/badge/IIIA-2-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2](https://img.shields.io/badge/IIIA-2-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3](https://img.shields.io/badge/IIIA-3-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-24](https://img.shields.io/badge/IIIA-24-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-25](https://img.shields.io/badge/IIIA-25-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **3** | [![IIIA-30](https://img.shields.io/badge/IIIA-30-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-31](https://img.shields.io/badge/IIIA-31-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3](https://img.shields.io/badge/IIIA-3-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3](https://img.shields.io/badge/IIIA-3-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4](https://img.shields.io/badge/IIIA-4-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-35](https://img.shields.io/badge/IIIA-35-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **4** | [![IIIA-40](https://img.shields.io/badge/IIIA-40-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-41](https://img.shields.io/badge/IIIA-41-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-42](https://img.shields.io/badge/IIIA-42-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4](https://img.shields.io/badge/IIIA-4-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4](https://img.shields.io/badge/IIIA-4-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5](https://img.shields.io/badge/IIIA-5-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **5** | [![IIIA-50](https://img.shields.io/badge/IIIA-50-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-51](https://img.shields.io/badge/IIIA-51-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-52](https://img.shields.io/badge/IIIA-52-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-53](https://img.shields.io/badge/IIIA-53-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5](https://img.shields.io/badge/IIIA-5-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5](https://img.shields.io/badge/IIIA-5-4D6BFE)](https://github.com/ErSanSan233/IIIA) |

### 全部等级（带星号）

作品以 AI 为主题时使用，同样 36 种：

| Z ＼ S | 0 | 1 | 2 | 3 | 4 | 5 |
| ------ | - | - | - | - | - | - |
| **0** | [![IIIA-0*](https://img.shields.io/badge/IIIA-0*-FAB689)](https://github.com/ErSanSan233/IIIA) | [![IIIA-1*](https://img.shields.io/badge/IIIA-1*-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-02*](https://img.shields.io/badge/IIIA-02*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-03*](https://img.shields.io/badge/IIIA-03*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-04*](https://img.shields.io/badge/IIIA-04*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-05*](https://img.shields.io/badge/IIIA-05*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **1** | [![IIIA-1*](https://img.shields.io/badge/IIIA-1*-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-1*](https://img.shields.io/badge/IIIA-1*-D9A295)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2*](https://img.shields.io/badge/IIIA-2*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-13*](https://img.shields.io/badge/IIIA-13*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-14*](https://img.shields.io/badge/IIIA-14*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-15*](https://img.shields.io/badge/IIIA-15*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **2** | [![IIIA-20*](https://img.shields.io/badge/IIIA-20*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2*](https://img.shields.io/badge/IIIA-2*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-2*](https://img.shields.io/badge/IIIA-2*-B97CAC)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3*](https://img.shields.io/badge/IIIA-3*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-24*](https://img.shields.io/badge/IIIA-24*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-25*](https://img.shields.io/badge/IIIA-25*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **3** | [![IIIA-30*](https://img.shields.io/badge/IIIA-30*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-31*](https://img.shields.io/badge/IIIA-31*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3*](https://img.shields.io/badge/IIIA-3*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-3*](https://img.shields.io/badge/IIIA-3*-A865B3)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4*](https://img.shields.io/badge/IIIA-4*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-35*](https://img.shields.io/badge/IIIA-35*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **4** | [![IIIA-40*](https://img.shields.io/badge/IIIA-40*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-41*](https://img.shields.io/badge/IIIA-41*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-42*](https://img.shields.io/badge/IIIA-42*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4*](https://img.shields.io/badge/IIIA-4*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-4*](https://img.shields.io/badge/IIIA-4*-9370DB)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5*](https://img.shields.io/badge/IIIA-5*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |
| **5** | [![IIIA-50*](https://img.shields.io/badge/IIIA-50*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-51*](https://img.shields.io/badge/IIIA-51*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-52*](https://img.shields.io/badge/IIIA-52*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-53*](https://img.shields.io/badge/IIIA-53*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5*](https://img.shields.io/badge/IIIA-5*-4D6BFE)](https://github.com/ErSanSan233/IIIA) | [![IIIA-5*](https://img.shields.io/badge/IIIA-5*-4D6BFE)](https://github.com/ErSanSan233/IIIA) |

---

## 贡献

如果您认为本等级标准存在不完善的地方，或者有更好的建议，欢迎通过提交 issue 或 pull request 的方式参与贡献。

当前版本对以下议题尤其欢迎讨论：两位数等级的贴纸方案、非视听类作品判定的边界情形、合成规则中阈值取 1 是否合适。

贴纸源文件为 pxd 格式，使用 Pixelmator Pro 制作。字体为狸叶黑体、阿里巴巴普惠体。

## 许可

本等级标准库采用 MIT 许可，您可以在遵循许可协议的前提下自由使用和传播。
