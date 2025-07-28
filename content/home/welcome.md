---
widget: blank
headless: false
weight: 10
title: Yu Lab
subtitle: Computational Biology and Ecology Laboratory

design:
  columns: '1'
  css_style: |
    /* 页面整体样式 */
    .yu-lab-page {
      font-family: 'Georgia', 'Times New Roman', serif;
      line-height: 1.6;
      color: #333;
    }

    /* 头部图片区域 */
    .lab-header {
      text-align: center;
      margin-bottom: 40px;
    }

    .lab-header img {
      max-width: 100%;
      height: 300px;
      object-fit: cover;
      border-radius: 12px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }

    .lab-header img:hover {
      transform: scale(1.02);
    }

    /* 实验室介绍 */
    .lab-intro {
      background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
      padding: 30px;
      border-radius: 12px;
      border-left: 5px solid #2c5aa0;
      margin-bottom: 40px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.08);
    }

    .lab-intro h3 {
      color: #2c5aa0;
      margin-bottom: 20px;
      font-size: 1.4em;
      font-weight: bold;
    }

    .lab-intro p {
      font-size: 1.1em;
      text-align: justify;
      margin-bottom: 15px;
    }

    /* 研究框架 */
    .research-framework {
      background: linear-gradient(135deg, #e8f2ff 0%, #f0f8ff 100%);
      padding: 30px;
      border-radius: 12px;
      margin-bottom: 40px;
      border: 2px solid #d0e7ff;
      text-align: center;
    }

    .research-framework h3 {
      color: #1a4480;
      font-size: 1.3em;
      margin-bottom: 15px;
      font-weight: bold;
    }

    .research-framework p {
      color: #2c5aa0;
      font-size: 1.1em;
      font-style: italic;
    }

    /* 三大支柱研究 */
    .pillar-research {
      margin-bottom: 50px;
    }

    .pillar-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
      gap: 30px;
      margin-top: 30px;
    }

    .pillar-card {
      background: white;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
      border-top: 5px solid #2c5aa0;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      position: relative;
    }

    .pillar-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 30px rgba(0,0,0,0.15);
    }

    .pillar-card::before {
      content: '';
      position: absolute;
      top: -5px;
      left: 0;
      right: 0;
      height: 5px;
      background: linear-gradient(90deg, #2c5aa0, #4CAF50, #FF9800);
      border-radius: 12px 12px 0 0;
    }

    .pillar-card h4 {
      color: #1a4480;
      margin-bottom: 10px;
      font-size: 1.3em;
      font-weight: bold;
    }

    .pillar-subtitle {
      color: #666;
      font-style: italic;
      margin-bottom: 20px;
      font-size: 0.95em;
    }

    .research-subarea {
      margin-bottom: 20px;
      padding: 15px;
      background: #f8f9fa;
      border-radius: 8px;
      border-left: 3px solid #2c5aa0;
    }

    .research-subarea h5 {
      color: #2c5aa0;
      margin-bottom: 8px;
      font-size: 1.1em;
      font-weight: bold;
    }

    .research-subarea ul {
      padding-left: 20px;
      margin: 0;
    }

    .research-subarea li {
      margin-bottom: 5px;
      color: #555;
      font-size: 0.95em;
    }

    /* 整合研究方法 */
    .integrated-approach {
      background: #f8f9fa;
      padding: 30px;
      border-radius: 12px;
      margin-bottom: 40px;
    }

    .integrated-approach h3 {
      color: #2c5aa0;
      text-align: center;
      margin-bottom: 25px;
      font-size: 1.5em;
    }

    .approach-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }

    .approach-item {
      background: white;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.05);
      border-left: 4px solid #4CAF50;
    }

    .approach-item h4 {
      color: #1a4480;
      margin-bottom: 10px;
      font-size: 1.1em;
    }

    .approach-item ul {
      padding-left: 15px;
      margin: 0;
    }

    .approach-item li {
      margin-bottom: 5px;
      color: #555;
      font-size: 0.9em;
    }

    /* 成果展示 */
    .achievements {
      background: #f8f9fa;
      padding: 30px;
      border-radius: 12px;
      margin-bottom: 40px;
    }

    .achievements h3 {
      color: #2c5aa0;
      text-align: center;
      margin-bottom: 25px;
      font-size: 1.5em;
    }

    .achievement-stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }

    .stat-item {
      text-align: center;
      padding: 20px;
      background: white;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.05);
    }

    .stat-number {
      font-size: 2em;
      font-weight: bold;
      color: #2c5aa0;
      display: block;
    }

    .stat-label {
      font-size: 0.9em;
      color: #666;
      margin-top: 5px;
    }

    /* 分隔线 */
    .section-divider {
      height: 3px;
      background: linear-gradient(to right, #2c5aa0, #e0e0e0, #2c5aa0);
      margin: 50px 0;
      border: none;
      border-radius: 2px;
    }

    /* 响应式设计 */
    @media (max-width: 768px) {
      .lab-header img {
        height: 200px;
      }

      .lab-intro, .research-framework, .integrated-approach {
        padding: 20px;
      }

      .pillar-grid {
        grid-template-columns: 1fr;
      }

      .pillar-card {
        padding: 20px;
      }

      .achievement-stats {
        grid-template-columns: repeat(2, 1fr);
      }

      .approach-grid {
        grid-template-columns: 1fr;
      }
    }
  css_class: yu-lab-page
---

<div class="lab-header">
  <img src="media/welcome.jpg" alt="Yu Lab - Computational Biology and Ecology Laboratory" />
</div>

<div class="lab-intro">
  <h3>About Yu Lab</h3>
  <p>The <strong> Computational Biology and Ecology Laboratory (Yu Lab)</strong> was founded in September 2020 and is based in the College of Life Science, Sichuan University (SCU), China. Led by Prof. YU Yan, who has been selected for the Ministry of Education's Major Talent Program for Young Scholars and serves as Deputy Director of the Southwest Bio-resources R&D Key Laboratory of Sichuan Province.</p>

  <p>At the interface between Biology and Computer Science, the lab is dedicated to understanding the evolutionary mysteries of life through big data and computational approaches. The team closely follows national strategic needs and has achieved significant breakthroughs in molecular marker extraction, theoretical methods for species origin and dispersal, and related tool development.</p>
</div>

<hr class="section-divider">

<div class="research-areas">
  <h2 style="text-align: center; color: #2c5aa0; font-size: 2em; margin-bottom: 10px;">Main Research Areas</h2>
  <p style="text-align: center; color: #666; font-size: 1.1em; margin-bottom: 30px;">Systematic Research on Biodiversity in Southwest China: From Morphological Classification to Model-Based Mechanisms</p>
  <div class="pillar-grid">
    <div class="pillar-card">
      <h3>1. Plant Classification Foundation</h3>
      <div class="research-subarea">
        <h4>Taxonomic Revision and Specimen Integration</h4>
        <ul>
          <li>Taxonomic revision of characteristic plant groups in Southwest China</li>
          <li>Construction of fundamental plant resource databases</li>
          <li>Morphological character analysis and standardization</li>
          <li>Herbarium specimen digitization and integration</li>
        </ul>
      </div>
      <div class="research-subarea">
        <h4>Biodiversity Survey and Documentation</h4>
        <ul>
          <li>Comprehensive floristic surveys in Southwest China</li>
          <li>Endemic species identification and characterization</li>
          <li>Rare and endangered species assessment</li>
          <li>Traditional taxonomic methodology optimization</li>
        </ul>
      </div>
    </div>
    <div class="pillar-card">
      <h3>2. Mechanism Research as Core</h3>
      <div class="research-subarea">
        <h5>Innovative Evolutionary Models</h5>
        <ul>
          <li>Development of multi-gene large-scale coalescent models</li>
          <li>Novel phylogenetic inference algorithms</li>
          <li>Evolutionary rate variation analysis</li>
          <li>Trait evolution modeling and simulation</li>
        </ul>
      </div>
      <div class="research-subarea">
        <h4>Biogeographic History Reconstruction</h4>
        <ul>
          <li>"Expansion-Extinction-Isolation" theoretical framework</li>
          <li>Historical climate change impact modeling</li>
          <li>Species dispersal pathway reconstruction</li>
          <li>Geological event correlation analysis</li>
        </ul>
      </div>
    </div>
    <div class="pillar-card">
      <h3>3. Resource Utilization as Guidance</h3>
      <div class="research-subarea">
        <h4>Gene Mining Methods Development</h4>
        <ul>
          <li>DBG (De Bruijn Graph) and weight-based hybrid sequence assembly models</li>
          <li>High-throughput sequencing data processing pipelines</li>
          <li>Functional gene identification and annotation</li>
          <li>Comparative genomics analysis tools</li>
        </ul>
      </div>
      <div class="research-subarea">
        <h4>Multi-omics Integration Tools</h4>
        <ul>
          <li>Transcriptome analysis software development</li>
          <li>Metabolome data integration platforms</li>
          <li>Proteome analysis workflows</li>
          <li>Multi-omics data visualization tools</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<hr class="section-divider">

<div style="background: linear-gradient(135deg, #e8f2ff 0%, #f0f8ff 100%); padding: 30px; border-radius: 12px; text-align: center; border: 2px solid #d0e7ff;">
  <h3 style="color: #2c5aa0; margin-bottom: 15px;">Research Philosophy</h3>
  <p style="font-size: 1.2em; font-style: italic; color: #1a4480; margin: 0;">
    <strong>"From Traditional Taxonomy to Computational Biology: Bridging Morphology and Mechanisms for Biodiversity Understanding"</strong>
  </p>
  <p style="margin-top: 15px; color: #666;">
    Committed to cultivating outstanding talents with interdisciplinary thinking and innovative capabilities, providing scientific basis for understanding biodiversity formation mechanisms and ecosystem dynamics
  </p>
</div>

<hr class="section-divider">

<div style="text-align: center; color: #666; font-style: italic;">
  <p><em>For more information, please visit our <a href="../research" style="color: #2c5aa0;">Research page</a> or <a href="../contact" style="color: #2c5aa0;">Contact us</a></em></p>
</div>
