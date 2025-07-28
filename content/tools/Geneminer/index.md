---
title: Geneminer

summary: A tool for extracting phylogenetic markers from next-generation sequencing data.

abstract: |
  Easy353 is a tool specifically designed to recover the Angiosperms353 gene set (AGS). It effectively filters AGS-related reads from high-throughput sequencing data, and accurately recovers AGS using its optimized reference-guided assembler.

# Schedule page publish date (NOT talk date).
publishDate: '2024-01-11T21:45:00Z'

authors:
  - Pulin Xie
  - Yongling Guo
  - Yan Yu

tags:
  - GeneMiner
  - NGS
  - Phylogenomics
  - Software

# Is this a featured talk? (true/false)
featured: true

image:
  caption: 'The workflow of Easy353'
  focal_point: Right

share: false  # Show social sharing links?

links:
  - name: GitHub
    url: https://github.com/sculab/GeneMiner
    icon_pack: fab
    icon: github

# url_code: ''
# url_pdf: ''
# url_slides: ''
# url_video: ''

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides:

# Projects (optional).
#   Associate this News with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
  - phylogenomics-tools
---

### 简介

测序技术的进步对进化生物学领域产生了革命性的影响，研究人员可以以非常低廉的价格获得大量的组学数据，从而获取多种对系统发育、进化和生态研究至关重要的分子标记。在生态学中，利用系统发育基因组学的分析方法进行关键生态性状的起源和演化、群落系统构建机制、物种多样化形成机制等问题的研究已是常规手段。研究者可以从核基因组、细胞器基因组、转录组等组学数据中获取丰富的分子标记，为目标类群建立系统发育树或网络，再结合形态学性状、生态因子、地质历史信息等，探索性状形成机制、群体进化历史、环境响应基因的生态适应与进化等。

使用组学数据进行系统发育分析可以产生大量的分子标记，从而获得更加丰富的系统发育信息。如何从组学数据中获取丰富且可靠分子标记，是系统发育方法学研究最基础也最重要的问题之一。然而，由于生态学的研究对象主要为非模式生物，缺少参考基因组且样本质量无法保证，使用现有的分析工具从组学数据，尤其是浅层测序数据中获取低拷贝核基因的成功率和准确度严重不足，导致对浅层测序数据的利用往往止步于质体基因和核糖体DNA（nrDNA）等高拷贝基因片段，大部分核基因的数据还未被有效利用

### 解决方案

四川大学余岩团队聚焦于系统发育标记挖掘的方法学研究，从过滤方法、组装算法和评估方法三个方面进行了探索：

1. Reads并行过滤模块：基于 k-mer 策略，在无需前处理实验的情况下高效提取目标基因相关序列。

2. 混合组装模块：基于参考序列构建加权 de Bruijn 图，从过滤后的 reads 中拼接得到准确的基因序列。

3. 组装校验模块：引入 parameter-bootstrap 重采样模型，有效降低参考序列变异对组装结果的干扰，提高稳定性和可重复性。

综合以上方法，研究人员开发了系统发育标记挖掘工具GeneMiner，并构建了两套的测试数据集：模式生物数据集(Arabidopsis thaliana和Oryza sativa)和模拟数据集进行验证，GeneMiner相对于同类工具在准确度、基因获取率和分析速度方面都表现出了明显的优势。

#### GeneMiner主要特点

* 能够从二代测序数据中大量提取用于系统发育分析的分子标记，相较于同类的工具拥有最高的提取率和准确率。
* 具有较强的通用型和鲁棒性，不仅能够用于转录组、重测序、富集测序等多类组学数据，对于低深度的测序数据也有较好的表现。 
* 提出了parameter-bootstrap校验方法，对于降低高变异参考序列对目标基因的影响非常有效，能够在很大程度排除不稳定的组装。 
* 运行速度快，对算力和内存的需求相对较低，既支持在高性能计算集群上并行运算，也可以在个人电脑上便捷的使用。 
* 对用户非常友好。支持Windows、macOS和Linux等主流的操作系统，用户可以选择命令行界面或图形界面进行使用。

GeneMiner能够优化系统发育基因组学研究过程，拓展研究范围，从方法学层面推动该领域的发展，推进生态学、进化生物学等相关学科的研究实践，加深对于生命演化机制的理解和认知，同时也为其他交叉学科领域提供理论支撑和研究工具，具有重要的理论价值和现实意义。

### 软件获取与版本说明

目前GeneMiner已经开发到2.1版本，为系统发育基因组学提供了全功能工具包，能够一站式完成从NGS数据获取到系统发育树建立的所有工作。

Windows用户推荐使用图形界面版本：GeneMiner2

GeneMiner2: a comprehensive analysis tool for the entire workflow from NGS raw data to phylogenetic tree construction.

命令行用户可选择：GeneMiner

GeneMiner: a software for extracting phylogenetic markers from next generation sequencing data.

