---
widget: blank
headless: true
active: true
weight: 10

title: ""
subtitle: ""

design:
  columns: '1'
  background:
    color: ''
    text_color_light: false
  spacing:
    padding: ["10px", "0", "20px", "0"]
  css_class: "research-page"
---

<style>
.research-page .research-intro {
  font-size: 1.1em;
  text-align: center;
  margin: 20px 0;
  padding: 20px;
  background-color: #f8f9fa;
  border-left: 4px solid #2c5aa0;
  border-radius: 4px;
}

.research-page .research-section {
  margin-bottom: 50px;
  padding: 25px;
  background-color: #f9f9f9;
  border-radius: 8px;
  border: 1px solid #e0e0e0;
}

.research-page .research-section p {
  text-align: justify;
  text-justify: inter-word;
  line-height: 1.6;
}

.research-page .research-section h3 {
  color: #1a4480 !important;
  margin-bottom: 15px;
  padding-left: 15px;
  border-left: 4px solid #2c5aa0;
}

.research-page .research-subsection {
  margin-bottom: 25px;
  padding: 15px;
  background-color: #ffffff;
  border-radius: 6px;
  border-left: 3px solid #4CAF50;
}

.research-page .research-subsection p {
  text-align: justify;
  text-justify: inter-word;
  line-height: 1.6;
}

.research-page .research-subsection h4 {
  color: #2c5aa0 !important;
  margin-bottom: 10px;
  font-size: 1.1em;
  font-weight: bold;
}

.research-page .key-finding {
  font-weight: bold;
  color: #1a4480;
}

.research-page .publication {
  font-style: italic;
  color: #666;
  margin-top: 15px;
  padding: 10px;
  background-color: #e8f2ff;
  border-radius: 4px;
  border-left: 3px solid #2c5aa0;
}

.research-page .methods-list {
  background-color: #f0f8ff;
  padding: 20px;
  border-radius: 8px;
  margin: 20px 0;
}

.research-page .methods-list p {
  text-align: justify;
  text-justify: inter-word;
  line-height: 1.6;
}

.research-page .methods-list ul {
  list-style: none;
  padding-left: 0;
}

.research-page .methods-list li {
  padding: 8px 0;
  border-bottom: 1px solid #e0e0e0;
}

.research-page .methods-list li:last-child {
  border-bottom: none;
}

.research-page .method-title {
  font-weight: bold;
  color: #2c5aa0;
}

.research-page .separator {
  height: 2px;
  background: linear-gradient(to right, #2c5aa0, #e0e0e0, #2c5aa0);
  margin: 40px 0;
  border: none;
}

.research-page .highlight-box {
  background-color: #e8f2ff;
  padding: 20px;
  border-radius: 8px;
  border-left: 4px solid #2c5aa0;
  margin: 20px 0;
}

.research-page .highlight-box p {
  text-align: justify;
  text-justify: inter-word;
  line-height: 1.6;
}

.research-page .framework-box {
  background: linear-gradient(135deg, #e8f2ff 0%, #f0f8ff 100%);
  padding: 25px;
  border-radius: 12px;
  margin-bottom: 30px;
  border: 2px solid #d0e7ff;
  text-align: center;
}

.research-page .framework-box h3 {
  color: #1a4480 !important;
  font-size: 1.2em;
  margin-bottom: 10px;
  font-weight: bold;
  border-left: none !important;
  padding-left: 0 !important;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .research-page .research-section {
    padding: 15px;
    margin-bottom: 30px;
  }
  
  .research-page .research-intro {
    padding: 15px;
    font-size: 1em;
  }
  
  .research-page .methods-list {
    padding: 15px;
  }
  
  .research-page .framework-box {
    padding: 15px;
  }
}
</style>

<div class="research-intro">
Our laboratory focuses on <strong>Computational Biology and Ecology</strong>, employing cutting-edge computational and molecular approaches to understand the evolutionary processes that shape biodiversity. We integrate genomic data with advanced phylogenetic methods to address fundamental questions in evolutionary biology.
</div>

<div class="framework-box">
  <h3>Research Framework</h3>
  <p style="color: #2c5aa0; font-style: italic; margin: 0;"><strong>Systematic Research on Biodiversity in Southwest China: From Morphological Classification to Model-Based Mechanisms</strong></p>
</div>

<hr class="separator">

## Research Areas

<div class="research-section">

### 1. Plant Classification Foundation

<div class="research-subsection">
<h4>Taxonomic Revision and Specimen Integration</h4>
<span class="key-finding">Traditional taxonomic methods combined with modern computational approaches form the foundation of our biodiversity research.</span> We conduct systematic taxonomic revision of characteristic plant groups in Southwest China, focusing on morphologically complex and taxonomically challenging groups. Our work includes construction of comprehensive plant resource databases, standardization of morphological character analysis, and large-scale digitization of herbarium specimens to create accessible digital collections for the scientific community.

<div class="publication">Key Publications:</div>
</div>

<div class="research-subsection">
<h4>Biodiversity Survey and Documentation</h4>
We conduct comprehensive floristic surveys across Southwest China's diverse ecosystems, from alpine meadows to tropical rainforests. Our fieldwork focuses on endemic species identification, rare and endangered species assessment, and documentation of previously unknown biodiversity hotspots. This work provides essential baseline data for conservation planning and evolutionary studies.

<div class="publication">Key Publications:</div>
</div>

</div>

<div class="research-section">

### 2. Mechanism Research as Core

<div class="research-subsection">
<h4>Innovative Evolutionary Models</h4>
<span class="key-finding">Development of multi-gene large-scale coalescent models represents a major advancement in phylogenetic inference.</span> We create novel algorithms that can handle massive genomic datasets while accounting for gene tree-species tree discordance, incomplete lineage sorting, and evolutionary rate variation. Our models incorporate both molecular and morphological data to provide more robust evolutionary hypotheses and better understand the mechanisms driving species diversification.

<div class="publication">Key Publications: Wen et al. 2020, Annals of Botany</div>
</div>

<div class="research-subsection">
<h4>Biogeographic History Reconstruction</h4>
Our "Expansion-Extinction-Isolation" theoretical framework provides new insights into how geological events and climate changes have shaped current biodiversity patterns. We develop sophisticated models that integrate paleoclimatic data, geological history, and molecular phylogenies to reconstruct species dispersal pathways and understand the timing of major evolutionary events in Southwest China.

<div class="publication">Key Publications: Yu et al. 2019, Molecular Biology and Evolution</div>
</div>

</div>

<div class="research-section">

### 3. Resource Utilization as Guidance

<div class="research-subsection">
<h4>Gene Mining Methods Development</h4>
<span class="key-finding">Our DBG (De Bruijn Graph) and weight-based hybrid sequence assembly models significantly improve the efficiency of genomic analysis.</span> We develop cutting-edge bioinformatics pipelines for processing high-throughput sequencing data, including novel approaches for functional gene identification, annotation, and comparative genomic analysis. These tools are specifically optimized for non-model organisms commonly found in Southwest China's biodiversity hotspots.

<div class="publication">Key Publications: Zhang et al. 2022, Molecular Biology and Evolution; Xie et al. 2024, Molecular Ecology Resources</div>
</div>

<div class="research-subsection">
<h4>Multi-omics Integration Tools</h4>
We create comprehensive software suites that integrate transcriptomic, metabolomic, and proteomic data to provide holistic views of biological systems. Our platforms include user-friendly interfaces for data visualization, statistical analysis, and interpretation, making advanced multi-omics analysis accessible to researchers studying biodiversity and evolution.

<div class="publication">Key Publications: Xie et al. 2024, Molecular Ecology Resources</div>
</div>

</div>

<hr class="separator">

## Research Methods & Approaches

<div class="methods-list">

Our research integrates multiple methodological approaches across the three pillars:

- <span class="method-title">Morphological Analysis:</span> Traditional taxonomic methods combined with geometric morphometrics and automated image analysis
- <span class="method-title">Phylogenetic Inference:</span> Advanced computational methods for reconstructing evolutionary relationships using multi-gene datasets
- <span class="method-title">Biogeographic Modeling:</span> Integration of molecular, climatic, and geological data to understand species distribution patterns
- <span class="method-title">Comparative Genomics:</span> Large-scale genome comparison to identify evolutionary innovations and adaptations
- <span class="method-title">Multi-omics Integration:</span> Combining genomic, transcriptomic, and metabolomic data for comprehensive biological understanding
- <span class="method-title">Conservation Genomics:</span> Application of genomic tools for biodiversity conservation and management strategies

</div>

<hr class="separator">

## Current Projects & Collaborations

<div class="highlight-box">
Our research is supported by major grants including National Natural Science Foundation of China, and involves collaborations with leading institutions worldwide. Current major projects include the Southwest China Biodiversity Genomics Initiative, the Digital Herbarium Platform, and the Conservation Genomics Program. We are committed to open science and making our data, tools, and computational resources available to the broader scientific community.
</div>

<hr class="separator">

*For more information about specific projects or potential collaborations, please [contact us](../contact).*
