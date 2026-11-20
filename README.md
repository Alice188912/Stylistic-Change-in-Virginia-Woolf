# Computational Literary Studies — 课程资料与研究成果

本仓库整理自 PhD courses / seminars / computational literary studies 课程文件夹（OSL 2023），包含课程阅读材料、实验语料、文体计量分析输出，以及课程论文草稿。

> 仓库为**私有**。课程阅读材料版权归各自作者所有；论文草稿为未发表内容，请勿公开分享。

## 整理说明

- 原始文件夹保持原样，未做任何修改；此处为整理后的副本。
- 按用途重新分组，文件名全部保留原样，便于与原始文件对应。
- 跳过了 Excel 临时锁文件 `~$frequencies.xlsx`。
- `Conrad_chance_1913.txt` 与 `Conrad_chance_1913(1).txt` 内容校验不同，因此两个版本均予以保留。
- `Monday or Tuesday 1921.txt` 与 `The-Waves 1931.txt` 在 `corpus/` 与 `final essay paper/` 中内容完全一致，合并为一份。
- 两处 `notes.docx` 内容不同：`final essay paper/` 中的版本保留在 `04-final-essay/`，顶层的版本放在 `01-course-materials/`。
- 共纳入 95 个源文件，另有本 README 与 `.gitignore`。

## 目录结构

| 目录 | 文件数 | 内容 |
| --- | ---: | --- |
| `01-course-materials/` | 16 | 课程手册、三次作业与配套阅读、AntConc / stylo 软件手册、顶层笔记 |
| `02-corpora/conrad/` | 25 | Conrad 小说与短篇文本语料（1895–1925） |
| `02-corpora/woolf/` | 14 | Virginia Woolf 作品语料（1915–1941），含论文用短篇 |
| `03-analysis-outputs/csv/` | 10 | 聚类 / 距离分析导出的边表与节点表 |
| `03-analysis-outputs/figures/` | 13 | CA、PCA、MDS 图表与词云截图 |
| `03-analysis-outputs/tables/` | 11 | 词频表、关键词 / KWIC 结果、距离表、stylometry 配置 |
| `04-final-essay/` | 6 | 课程论文草稿、笔记、参考论文与补充材料 |

## 各目录详情

### 01-course-materials

课程手册、CLS 1–3 的作业与阅读文献（Burrows 的 Delta 方法、McCarthy & Sullivan 的语料文体学、Plath / Sexton 研究、Boot & Koolen、Riddell 等），以及 AntConc、stylometry 工具的使用说明。

### 02-corpora

- `conrad/`：来自 CLS experiments/Corpus 的 Conrad 作品纯文本。
- `woolf/`：来自 corpus/ 目录的 Woolf 长篇与短篇，另含 final essay paper 中用于对比分析的 6 篇短篇文本。

### 03-analysis-outputs

按文件格式分为三类：

- `csv/`：Classic Delta、Consensus（wurzburg）、MDS 等方法的 EDGES / NODES 文件，参数写在文件名中（如 MFWs 数量、Culled 值、聚类阈值）。
- `figures/`：对应分析的可视化图像，包含论文中的图表和词云。
- `tables/`：AntConc 导出的关键词、KWIC、词表、词频表，以及 stylo 配置文件。

### 04-final-essay

课程论文相关文档：`final essay draft.docx`、`final May 8.docx`、`notes.docx`，以及 Vogel 关于研究工具的文章、印象主义文学运动参考资料等 PDF。

## 复现提示

分析输出由 R 的 `stylo` 包与 AntConc 生成。参数可从文件名与 `03-analysis-outputs/tables/stylo_config.txt` 中读取。
