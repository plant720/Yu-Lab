---
title: MetaGeneminer

summary: A tool for targeted gene extraction and assembly from metagenomic sequencing data.

abstract: |
  MetaGeneMiner is a user-friendly software tool designed to extract and assemble target genes from metagenomic sequencing data. It employs a three-module architecture for k-mer-based read filtering, optimal reference selection, and guided assembly. The tool has been validated in clinical datasets for antimicrobial resistance (AMR) gene detection, providing a rapid and cost-effective solution for resistance surveillance and molecular epidemiology.

# Schedule page publish date (NOT talk date).
publishDate: '2024-07-05T00:00:00Z'

authors:
  - Zizhen Tang
  - Yan Yu

tags:
  - Easy353
  - Angiosperms353
  - Phylogenomics
  - Software

# Is this a featured talk? (true/false)
featured: true

image:
  caption: 'The workflow of MetaGeneMiner'
  focal_point: Right

share: false  # Show social sharing links?

links:
  - name: Gitee
    url: https://gitee.com/sculab/MetaGeneMiner
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

由于抗生素误用和滥用现象的不断发生，微生物的抗生素耐药性在近年来成为日益严峻的公共卫生问题。在美国，抗生素耐药性感染每年导致了超过200亿美元的额外医疗支出。为了控制抗生素耐药性的扩散，亟需建立一套耐药性监控体系，在病原微生物中检测并追踪抗生素耐药性的传播和发展。然而，药物敏感性试验需要较长时间才能完成，限制了对抗生素耐药性的大规模检测。随着测序技术的快速发展，宏基因组测序的通量不断提高，允许研究人员对抗生素耐药基因实现大范围、低成本的检测。在这一背景下，数据分析软件的易用性和计算速度成为了扩展抗生素耐药性检测覆盖范围的关键因素。

该研究设计了三个软件模块用于实现宏基因组数据的高效提取：读段过滤模块基于k-mer匹配，在原始测序数据中筛选与目标基因相关的读段；最优参考选择模块根据读段过滤的结果，选取能够实现最高质量组装的参考序列；基于参考序列的组装模块组装最终的基因序列，使用户能够获得所需基因的具体序列数据。在这三个软件模块的基础上，本文设计了一个高效且用户友好的图形界面，并构建了MetaGeneMiner软件包，允许用户在主流配置的个人电脑上对大量的宏基因组数据进行分析，大幅简化了耐药性基因进行检测的流程。

MetaGeneMiner在临床数据上表现出了较好的性能。在鲍曼不动杆菌已知的1974个基因中，MetaGeneMiner在最少的样本中也还原出了1645个，且处理四个样本的运行时间小于两小时。在所有样本中，MetaGeneMiner组装出的抗生素耐药性基因包含了AMR++管线找到的所有耐药性基因，证明了MetaGeneMiner能够从宏基因组数据中高效地提取并组装基因。

该研究开发并验证了MetaGeneMiner，一种从宏基因组中针对性提取并组装基因序列的工具。MetaGeneMiner简化了从宏基因组测序数据中检测抗生素耐药基因的流程，提供了一种对抗生素耐药性进行监测的简便途径。作为一个通用工具，MetaGeneMiner表现出了多个领域中的应用潜力，包括：环境微生物学、生物信息学、基因组学和流行病学。

MetaGeneMiner易于安装，提供了用户友好的图形界面，并且可以在所有流行的操作系统上运行。特别是对于Windows用户，设计了一个先进的图形界面工具，该工具具有便携性，大大简化了用户体验并扩展了工具的可访问性，软件和源代码可以访问https://gitee.com/sculab/MetaGeneMiner。
