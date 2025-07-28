---
title: Easy353

summary: A tool specifically designed to recover the Angiosperms353 gene set (AGS).

abstract: |
  Easy353 is a tool specifically designed to recover the Angiosperms353 gene set (AGS). It effectively filters AGS-related reads from high-throughput sequencing data, and accurately recovers AGS using its optimized reference-guided assembler.

# Schedule page publish date (NOT talk date).
publishDate: '2023-08-14T00:00:00Z'

authors:
  - Zhen Zhang
  - Yan Yu
  - Pulin Xie
  - Yongling Guo

tags:
  - Easy353
  - Angiosperms353
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
    url: https://github.com/plant720/Easy353
    icon_pack: fab
    icon: github
  - name: Documentation
    url: https://github.com/plant720/Easy353/wiki
    icon_pack: fas
    icon: book

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

为了从各种测序数据中高效准确的获取以AGS为代表的低拷贝基因，四川大学生命科学学院余岩教授团队开发了Easy353工具包，能够直接从包括浅层基因组测序的各类高通量测序中获取AGS等低拷贝基因。

Easy353是基于reference-guided策略的拼接工具，使用de Bruijn graph的算法进行有权重的从头拼接，具有极高的准确性和敏感度。该工具使用流程比较简单，研究者无需进行任何前置实验，仅仅提供同科/属的参考序列和测序的原始数据就可以直接获取各类低拷贝/单拷贝基因。

为了方便研究者使用，Easy353同时支持Linux、MacOS、Windows系统，并为Windows和MacOS提供了用户图形界面。该工具包可在 [GitHub](https://github.com/plant720/Easy353) 上免费获取使用。

Easy353简单易用，能够让用户在较短的时间内，利用低成本低深度的数据获得高质量的系统发育标记（DNA条码），能够大幅度减少重复工作和复杂的实验，有利于研究人员开展相关工作，推动相关学科的高质量快速发展。
