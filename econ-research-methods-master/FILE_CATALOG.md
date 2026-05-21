# Gitee Repository File Catalog

**Repository**: [econ-research-methods](https://gitee.com/zhiyuanryanchen/econ-research-methods)  
**Total files**: 384  
**Last updated**: 2026-04-16

---

## 仓库结构总览 (Directory Tree)

```
econ-research-methods/
├── LICENSE
├── README.md
├── FILE_CATALOG.md
│
├── .gitee/                              # Gitee 平台模板
│   ├── ISSUE_TEMPLATE.en.md
│   └── PULL_REQUEST_TEMPLATE.en.md
│
├── 2020Fall/                            # 2020 秋季学期
│   ├── EconResearchMethods2020Syllabus.pdf
│   ├── Lecture1/                        # 数据获取与可视化
│   │   ├── 1-WebScrapping/              #   网页爬虫
│   │   │   └── nbsPdtCode_TrialCodes.ipynb
│   │   ├── 2-DataVisualization/         #   数据可视化
│   │   │   ├── Patent_Tracks_Analysis.ipynb
│   │   │   ├── Stata_Example_Jupyter.ipynb
│   │   │   └── visualization_rules.ipynb
│   │   ├── 3-StataJupyter/             #   Stata + Jupyter
│   │   │   ├── Project_Example_MixedFacts.ipynb
│   │   │   ├── stata_example.do
│   │   │   └── Stata_Jupyter.ipynb
│   │   └── Gitee使用教程.pdf
│   ├── Lecture2/                        # 面板数据与因果推断
│   │   └── L2_panel_causal.pdf
│   ├── Lecture3/                        # Stata 编程
│   │   ├── 4-PanelModels/              #   面板模型 & DID
│   │   │   ├── DiffinDiff.ipynb
│   │   │   ├── PanelModels.ipynb
│   │   │   └── *.dta, *.gph            #   数据文件
│   │   ├── 5-UsingStataResults/        #   e-class / r-class
│   │   │   └── Results_e-class_r-class.ipynb
│   │   ├── 6-AdvancedProgramming/      #   高级编程
│   │   │   └── AdvancedProgramming.ipynb
│   │   ├── 7-BootstrapMethods/         #   Bootstrap 方法
│   │   │   ├── BootstrapMethods.ipynb
│   │   │   └── *.dta                   #   数据文件
│   │   ├── 8-Simulation/              #   蒙特卡洛模拟
│   │   │   ├── MonteCarloSimulations.ipynb
│   │   │   └── *.dta
│   │   └── 9-MatalabIntro/            #   MATLAB 入门
│   │       ├── MatlabIntro.ipynb
│   │       ├── MatlabIntro.mlx
│   │       ├── SolveLinearSystem.mlx
│   │       ├── IntroScript.m
│   │       └── circlefn.m
│   ├── Lecture4/                        # 机器学习与文本分析
│   │   ├── L4-MLeconomics.pdf
│   │   └── 10-TextAnalysis/            #   中文文本分析
│   │       ├── ChineseTextAnalysisIntro.ipynb
│   │       └── *.txt                   #   停用词 & 词典
│   ├── Lecture5/                        # 理论方法
│   │   └── L5-theory.pdf
│   ├── Lecture6/                        # 数值方法与引力模型
│   │   ├── 11-SolvingNonLinearSystem/  #   非线性方程求解
│   │   │   ├── SolvingNonLinearSystem.ipynb
│   │   │   └── *.m                     #   MATLAB 函数
│   │   └── 12-Gravity/                 #   引力模型估计
│   │       ├── GravityEstimation.ipynb
│   │       ├── gravity_main.m
│   │       └── trdata.mat
│   └── Lecture7/                        # 需求估计 (BLP)
│       ├── 13-BLP/                     #   BLP Stata 实现
│       │   ├── BLP.ipynb
│       │   ├── BLP_Stata.ipynb
│       │   └── *.dta, *.do
│       └── BLP-Code/                   #   BLP MATLAB 实现
│           ├── example.m
│           ├── readme.md
│           └── *.m (14 files)          #   完整 BLP 求解器
│
├── 2022Spring/                          # 2022 春季学期
│   ├── RMEB2022Spring_Syllabus.pdf
│   ├── L1-CausalInference/
│   │   └── 1-CausalInference.pdf
│   └── L2-Panel-DID/
│       ├── L2_PanelModels_DID.pdf
│       └── L3_More_DID.pdf
│
├── 2025Spring/                          # 2025 春季学期
│   ├── RMEB2025Spring_Syllabus.pdf
│   ├── Lecture Notes/                   # 讲义（11讲）
│   │   ├── 第一讲-Causal Inference Intro-RMEB2025Spring.pdf
│   │   ├── 第二讲-Linear Regressions-RMEB2025Spring.pdf
│   │   ├── S1-Shift-Share IV-RMEB2025Spring.pdf
│   │   ├── S2-Classical Regressions-RMEB2025Spring.ipynb
│   │   ├── S3-Penalized-Linear-Regressions.ipynb
│   │   ├── 第三讲_PanelData_RMEB2025Spring.pdf
│   │   ├── 第四讲-More On DiD-RMED2025Spring.pdf
│   │   ├── 第五讲-Diff-In-Diffs in Dynamic Models.pdf
│   │   ├── S4-Tree-Based Methods-Python-Application.ipynb
│   │   ├── 第六讲-Machine Learning Intro-RMEB2025Spring.ipynb
│   │   ├── 第七讲-Tree-Based Methods.ipynb
│   │   ├── 第八讲-CausalForest.pdf
│   │   ├── 第九讲-Algorithms_StructuralEstimation.ipynb
│   │   ├── 第十讲-Deep_Learning.ipynb
│   │   ├── 第十一讲-NLP.ipynb
│   │   └── images/                     #   讲义配图（37张）
│   │       ├── *.png, *.jpg, *.webp
│   │       └── (神经网络、Transformer、专利质量等)
│   ├── Assignments/                     # 作业
│   │   ├── Assignment 1.ipynb
│   │   ├── Programming Practice 1-Monte Carlo Simulation-Clustered SE.ipynb
│   │   └── estimation_sample.csv
│   ├── Code Notebooks/                  # 代码练习
│   │   ├── causal_forest_econml.ipynb   #   EconML 因果森林
│   │   ├── causal_forest_grf_guide.Rmd  #   grf R 指南
│   │   ├── HonestDiD.Rmd               #   Honest DID (R)
│   │   ├── jackknife_bootstrap_method.ipynb
│   │   ├── Practice 1-Various Diff-In-Diffs Estimators.ipynb
│   │   └── R_intro.R
│   └── Readings/                        # 阅读材料（10篇）
│       ├── AI for research-Nature2025.pdf
│       ├── DiD_Review_Paper.pdf
│       ├── DoublyRobustMachineLearning.pdf
│       ├── PolicyLearning-AtheyWager2021ECTA.pdf
│       └── ... (共10篇论文)
│
├── 2026Spring/                          # 2026 春季学期（待填充）
│
└── empirical_methods_book/              # Jupyter Book 教材项目
    └── Empirical Methods for Economic Studies/
        ├── _config.yml                  #   Jupyter Book 配置
        ├── _toc.yml                     #   目录结构
        ├── intro.md                     #   引言
        ├── Machine-Learning-Intro.ipynb #   机器学习入门
        ├── markdown-notebooks.md        #   Markdown 笔记本示例
        ├── markdown.md                  #   Markdown 示例
        ├── notebooks.ipynb              #   Notebook 示例
        ├── references.bib              #   参考文献
        ├── requirements.txt            #   依赖
        ├── logo.png                    #   Logo
        └── _build/                     #   构建产物（HTML站点）
            ├── html/                   #     HTML 输出
            └── jupyter_execute/        #     执行缓存
```

### 学期内容演进

| 学期 | 核心内容 | 编程语言 | 材料形式 |
|------|---------|---------|---------|
| **2020 秋** | 数据获取、面板模型、DID、Bootstrap、蒙特卡洛、文本分析、引力模型、BLP | Stata, Python, MATLAB | Jupyter Notebook + PDF 讲义 |
| **2022 春** | 因果推断、面板数据 & DID | — | PDF 讲义 |
| **2025 春** | 因果推断、回归、正则化、DID、机器学习、因果森林、结构估计、深度学习、NLP | Python, R, Stata | Jupyter Notebook + PDF 讲义 |
| **2026 春** | *(开发中)* | — | Quarto RevealJS |

---

## Root

| File | Description |
|------|-------------|
| `LICENSE` | License file |
| `README.md` | Repository introduction and course description |

---

## `.gitee/`

Gitee platform templates.

| File | Description |
|------|-------------|
| `ISSUE_TEMPLATE.en.md` | Issue template (English) |
| `PULL_REQUEST_TEMPLATE.en.md` | Pull request template (English) |

---

## `2020Fall/`

2020 秋季学期课程材料。

| File | Description |
|------|-------------|
| `EconResearchMethods2020Syllabus.pdf` | 2020秋季教学大纲 |

### `2020Fall/Lecture1/` — 数据获取与可视化

#### `1-WebScrapping/`
| File | Description |
|------|-------------|
| `nbsPdtCode_TrialCodes.ipynb` | 网页爬虫示例代码 |

#### `2-DataVisualization/`
| File | Description |
|------|-------------|
| `Patent_Tracks_Analysis.ipynb` | 专利轨迹分析可视化 |
| `Stata_Example_Jupyter.ipynb` | Stata Jupyter示例 |
| `visualization_rules.ipynb` | 数据可视化规则 |

#### `3-StataJupyter/`
| File | Description |
|------|-------------|
| `Project_Example_MixedFacts.ipynb` | 项目示例 |
| `stata_example.do` | Stata do-file示例 |
| `Stata_Jupyter.ipynb` | Stata + Jupyter集成示例 |

| Other | |
|-------|---|
| `Gitee使用教程.pdf` | Gitee平台使用教程 |

### `2020Fall/Lecture2/` — 面板数据与因果推断

| File | Description |
|------|-------------|
| `L2_panel_causal.pdf` | 面板数据与因果推断讲义 |

### `2020Fall/Lecture3/` — 编程与模拟

#### `4-PanelModels/`
| File | Description |
|------|-------------|
| `DiffinDiff.ipynb` | 双重差分（DID）实现 |
| `PanelModels.ipynb` | 面板模型实现 |
| `Panel101.dta` | 面板数据示例 |
| `mus08psidextract.dta` | PSID数据提取 |
| `outsourcingatwill_table7.zip` | 外包数据（压缩包） |
| `lwage_ts.gph` / `wks_ts.gph` | Stata图形文件 |

#### `5-UsingStataResults/`
| File | Description |
|------|-------------|
| `Results_e-class_r-class.ipynb` | Stata e-class/r-class结果处理 |

#### `6-AdvancedProgramming/`
| File | Description |
|------|-------------|
| `AdvancedProgramming.ipynb` | 高级编程技术 |

#### `7-BootstrapMethods/`
| File | Description |
|------|-------------|
| `BootstrapMethods.ipynb` | Bootstrap方法实现 |
| `bootmean.dta` / `uniform_sample.dta` / `usample.dta` | 示例数据文件 |

#### `8-Simulation/`
| File | Description |
|------|-------------|
| `MonteCarloSimulations.ipynb` | 蒙特卡洛模拟 |
| `mcs.dta` / `mcsimulate.dta` | 模拟数据文件 |

#### `9-MatalabIntro/`
| File | Description |
|------|-------------|
| `MatlabIntro.ipynb` | MATLAB入门（Jupyter） |
| `MatlabIntro.mlx` | MATLAB入门（Live Script） |
| `SolveLinearSystem.mlx` | 线性方程组求解 |
| `IntroScript.m` | 入门脚本 |
| `circlefn.m` | 圆函数示例 |

### `2020Fall/Lecture4/` — 机器学习与文本分析

#### `10-TextAnalysis/`
| File | Description |
|------|-------------|
| `ChineseTextAnalysisIntro.ipynb` | 中文文本分析入门 |
| `text.txt` | 示例文本 |
| `stop_words.txt` / `user_stopwords.txt` | 停用词表 |
| `userdict.txt` / `userdict_lac.txt` | 用户词典 |

| Other | |
|-------|---|
| `L4-MLeconomics.pdf` | 机器学习与经济学讲义 |

### `2020Fall/Lecture5/` — 理论

| File | Description |
|------|-------------|
| `L5-theory.pdf` | 理论讲义 |

### `2020Fall/Lecture6/` — 非线性系统与引力模型

#### `11-SolvingNonLinearSystem/`
| File | Description |
|------|-------------|
| `SolvingNonLinearSystem.ipynb` | 非线性方程组求解 |
| `bisection.m` | 二分法 |
| `cournot.m` | Cournot模型 |
| `myJac.m` | 雅可比矩阵计算 |
| `NewtonIteration_Ani.gif` | 牛顿迭代动画 |

#### `12-Gravity/`
| File | Description |
|------|-------------|
| `GravityEstimation.ipynb` | 引力模型估计 |
| `gravity_main.m` | 引力模型主程序 |
| `gravity_estobj.m` | 估计目标函数 |
| `gravity_priobj.m` | 先验目标函数 |
| `trdata.mat` | 贸易数据 |
| `main_est.out` / `main-est.out` | 估计输出 |

### `2020Fall/Lecture7/` — BLP需求估计

#### `13-BLP/`
| File | Description |
|------|-------------|
| `BLP.ipynb` | BLP模型（Python） |
| `BLP_Stata.ipynb` | BLP模型（Stata） |
| `blp_demo.do` | BLP Stata do-file |
| `blp_demo.dta` / `blp_nodemo.dta` / `demodata.dta` | BLP数据文件 |
| `blp_stata_command.jpg` | Stata命令截图 |

#### `BLP-Code/`
| File | Description |
|------|-------------|
| `readme.md` | BLP代码说明 |
| `example.m` | 主程序入口 |
| `example.diary` | 运行日志 |
| `sample.mat` | 样本数据 |
| `solveRCBLPpar.m` | 随机系数BLP求解器 |
| `solveAllShares.m` | 市场份额求解 |
| `solveNewton.m` | 牛顿法求解器 |
| `fp_squarem.m` | SQUAREM不动点加速 |
| `rc_share_safe.m` | 随机系数份额计算 |
| `RCBLP_Jacobian.m` | 雅可比矩阵 |
| `ivregression.m` | IV回归 |
| `extract_params.m` | 参数提取 |
| `print_results.m` | 结果打印 |
| `finite_difference.m` | 有限差分 |
| `myDerivCheck.m` | 导数检查 |
| `correlated_normal.m` | 相关正态分布 |
| `indep_normal.m` | 独立正态分布 |

---

## `2022Spring/`

2022 春季学期课程材料。

| File | Description |
|------|-------------|
| `RMEB2022Spring_Syllabus.pdf` | 2022春季教学大纲 |

### `2022Spring/L1-CausalInference/`
| File | Description |
|------|-------------|
| `1-CausalInference.pdf` | 因果推断讲义 |

### `2022Spring/L2-Panel-DID/`
| File | Description |
|------|-------------|
| `L2_PanelModels_DID.pdf` | 面板模型与DID讲义 |
| `L3_More_DID.pdf` | 更多DID方法讲义 |

---

## `2025Spring/`

2025 春季学期课程材料。

| File | Description |
|------|-------------|
| `RMEB2025Spring_Syllabus.pdf` | 2025春季教学大纲 |

### `2025Spring/Lecture Notes/` — 讲义

| File | Description |
|------|-------------|
| `第一讲-Causal Inference Intro-RMEB2025Spring.pdf` | 第1讲：因果推断导论 |
| `第二讲-Linear Regressions-RMEB2025Spring.pdf` | 第2讲：线性回归 |
| `S2-Classical Regressions-RMEB2025Spring.ipynb` | 第2讲：经典回归（Notebook） |
| `第三讲_PanelData_RMEB2025Spring.pdf` | 第3讲：面板数据 |
| `第四讲-More On DiD-RMED2025Spring.pdf` | 第4讲：更多DID方法 |
| `第五讲-Diff-In-Diffs in Dynamic Models.pdf` | 第5讲：动态DID |
| `S1-Shift-Share IV-RMEB2025Spring.pdf` | Shift-Share IV |
| `第六讲-Machine Learning Intro-RMEB2025Spring.ipynb` | 第6讲：机器学习入门 |
| `S3-Penalized-Linear-Regressions.ipynb` | 惩罚线性回归 |
| `第七讲-Tree-Based Methods.ipynb` | 第7讲：树模型方法 |
| `S4-Tree-Based Methods-Python-Application.ipynb` | 树模型Python应用 |
| `第八讲-CausalForest.pdf` | 第8讲：因果森林 |
| `第九讲-Algorithms_StructuralEstimation.ipynb` | 第9讲：算法与结构估计 |
| `第十讲-Deep_Learning.ipynb` | 第10讲：深度学习 |
| `第十讲-Deep_Learning.html` | 第10讲：深度学习（HTML） |
| `第十一讲-NLP.ipynb` | 第11讲：自然语言处理 |

### `2025Spring/Lecture Notes/images/` — 讲义图片

共 37 张图片，涵盖神经网络架构、注意力机制、Transformer、词嵌入、专利分析等。

| File | Description |
|------|-------------|
| `a_single_neuron.png` | 单个神经元示意图 |
| `activation_functions.png` | 激活函数 |
| `Adam_algorithm.png` | Adam优化算法 |
| `attention_paper_impact.png` | 注意力论文影响力 |
| `backdrop_example_z14.png` / `backdrop_simple_example.png` | 反向传播示例 |
| `backpro_compute_example.png` / `backpro_compute1.png` / `backpro_compute2.png` | 反向传播计算 |
| `bert_wwm_job_classification_performance.png` | BERT分类性能 |
| `breakthrough_patents.png` | 突破性专利 |
| `chapter03_attention-ops.png` | 注意力操作 |
| `chapter03_contextualized-embedding.png` | 上下文嵌入 |
| `chapter03_decoder-zoom.png` / `chapter03_encoder-zoom.png` | 编解码器细节 |
| `chapter03_layer-norm.png` | 层归一化 |
| `chapter03_multihead-attention.png` | 多头注意力 |
| `chapter03_transformer-encoder-decoder.png` | Transformer编解码器 |
| `chapter03_transformers-compact.png` | Transformer紧凑图 |
| `computation_graphs_backpro.png` / `computation_graphs.png` | 计算图 |
| `Finbert_accuracy.png` | FinBERT准确率 |
| `HM_social_system.png` | 社会系统模拟 |
| `intuitive_tensor.png` | 张量直觉 |
| `IP_textcounts.png` | 知识产权文本统计 |
| `LSTM_structure.webp` | LSTM结构 |
| `neural_network_two_layers.png` / `neural-network-architecture.png` | 神经网络架构 |
| `neurons.jpg` | 神经元 |
| `non-linear_classifier.png` | 非线性分类器 |
| `occupation_technology_exposure.png` | 职业技术暴露 |
| `pairwise_patent_similarity.png` | 专利相似度 |
| `RNNs_training.png` / `RNNs.webp` | RNN训练与结构 |
| `sequence_to_sequence_attention_final.png` | Seq2Seq注意力（最终） |
| `sequence_to_sequence_attention1.png` / `attention2.png` / `attention3.png` | Seq2Seq注意力（步骤） |
| `single_node_backpro.png` / `single_node_backpro_conti.png` | 单节点反向传播 |
| `transformer_architecture.png` | Transformer架构 |
| `word2vec_model.png` | Word2Vec模型 |
| `WordEmbeddings.jpg` | 词嵌入 |
| `不同主体专利质量与数量.png` | 不同主体专利质量与数量 |
| `不同专利质量指标相关性.png` | 不同专利质量指标相关性 |
| `中外专利质量对比变化.png` | 中外专利质量对比变化 |

### `2025Spring/Assignments/` — 作业

| File | Description |
|------|-------------|
| `Assignment 1.ipynb` | 作业1（Notebook） |
| `Assignment 1.html` | 作业1（HTML） |
| `estimation_sample.csv` | 估计样本数据 |
| `Programming Practice 1-Monte Carlo Simulation-Clustered SE.ipynb` | 编程练习1：蒙特卡洛模拟与聚类标准误 |
| `Programming Practice 1-Monte Carlo Simulation-Clustered SE.html` | 编程练习1（HTML） |

### `2025Spring/Code Notebooks/` — 代码笔记本

| File | Description |
|------|-------------|
| `causal_forest_econml.ipynb` | 因果森林 (EconML) |
| `causal_forest_grf_guide.Rmd` | 因果森林 (grf) R指南 |
| `HonestDiD.Rmd` | Honest DID (R) |
| `jackknife_bootstrap_method.ipynb` | Jackknife与Bootstrap方法 |
| `Practice 1-Various Diff-In-Diffs Estimators.ipynb` | 各种DID估计量 |
| `R_intro.R` | R语言入门 |

### `2025Spring/Readings/` — 阅读材料

| File | Description |
|------|-------------|
| `AI for research-Nature2025.pdf` | AI与研究 (Nature 2025) |
| `Athey-Estimating Treatment Effects with Causal Forests-2019.pdf` | Athey因果森林论文 |
| `Banerjee et al-2020-A Theory of Experimenters.pdf` | Banerjee实验者理论 |
| `DiD_Review_Paper.pdf` | DID综述论文 |
| `DoublyRobustMachineLearning.pdf` | 双重稳健机器学习 |
| `GoldsmithPinkham-BartikInstruments-2020.pdf` | Bartik工具变量 |
| `Higbee-Experimental Design for Policy Choice.pdf` | 政策选择实验设计 |
| `HumanSocietySimulation-tutorial-LLM4Simu.pdf` | LLM社会模拟教程 |
| `JMP_TG.pdf` | JMP论文 |
| `PolicyLearning-AtheyWager2021ECTA.pdf` | 政策学习 (Athey & Wager 2021) |
| `Wang和Yang-Policy Experimentation in China.pdf` | 中国政策实验 |

---

## `2026Spring/`

2026 春季学期课程材料（当前学期）。

> **注意**：此目录在Gitee仓库中目前为空或仅包含占位文件。  
> 当前学期的主要内容通过 GitHub Pages 网站发布。

---

## `empirical_methods_book/`

Jupyter Book 项目：*Empirical Methods for Economic Studies*。

### Source Files

| File | Description |
|------|-------------|
| `_config.yml` | Jupyter Book配置 |
| `_toc.yml` | 目录结构 |
| `intro.md` | 书籍导言 |
| `markdown.md` | Markdown示例 |
| `markdown-notebooks.md` | Markdown笔记本示例 |
| `notebooks.ipynb` | Jupyter笔记本示例 |
| `Machine-Learning-Intro.ipynb` | 机器学习入门章节 |
| `references.bib` | 参考文献 |
| `requirements.txt` | Python依赖 |
| `logo.png` | 书籍Logo |

### Build Output (`_build/`)

Built HTML site with Sphinx Book Theme. Contains:

- **`_build/html/`** — Rendered HTML pages (`intro.html`, `Machine-Learning-Intro.html`, `markdown.html`, `notebooks.html`, etc.)
- **`_build/html/_static/`** — Static assets (CSS, JS, fonts, icons, locale files for 30+ languages)
- **`_build/html/_sources/`** — Source copies
- **`_build/jupyter_execute/`** — Executed notebook outputs
- **`_build/.doctrees/`** — Sphinx doctree cache

---

## File Type Summary

| Type | Count | Description |
|------|-------|-------------|
| `.ipynb` | ~30 | Jupyter Notebooks (Python, Stata, MATLAB) |
| `.pdf` | ~20 | Lecture slides and readings |
| `.m` | ~18 | MATLAB scripts |
| `.dta` | ~8 | Stata data files |
| `.html` | ~15 | Rendered HTML pages |
| `.py` / `.R` / `.Rmd` / `.do` | ~5 | Code scripts |
| `.png` / `.jpg` / `.gif` / `.webp` | ~45 | Images and figures |
| `.css` / `.js` | ~30 | Web static assets (Jupyter Book) |
| `.md` | ~8 | Markdown documents |
| Other | ~205 | Build artifacts, locale files, fonts, config |
