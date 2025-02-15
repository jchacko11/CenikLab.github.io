---
layout: page
title: A computational ecosystem to understand translational control
html: True
permalink: /lab_research-ribo-ecosystem
summary: We have designed a dedicated binary hierarchical data format to efficiently store, organize and process ribosome profiling data, as well as a computational ecosystem around it.
---

<center>
<!-- <h1> A computational ecosystem to understand translation</h1> -->
</center>

<p>
  <center>
  <img src="/img/publications/2020_bioinfomatics.jpg" alt="Ribo Ecosystem" style="width:400px;">
  </center>
</p>

mRNA translation can be measured transcriptome-wide by sequencing of mRNA
fragments protected by ribosomes from RNase digestion.
This approach, called ribosome profiling,
poses unique computational challenges.
Unlike RNA sequencing measurements,
ribosome profiling data typically needs to be analyzed
as a function of the read/footprint size.
This results in significant bottlenecks in storage and processing,
as many values need to be stored for each gene and experiment.
While there are specialized solutions for other data modalities
such as <a href="https://samtools.github.io/hts-specs/SAMv1.pdf">BAM</a> for sequence alignment,
or <a href="https://cooler.readthedocs.io/en/latest/datamodel.html">Cooler</a> /
<a href="https://github.com/aidenlab/juicer/wiki/Data">hic</a> for chromosome conformation capture  data,
ribosome profiling experiments lacked a comparable dedicated and standardized format.
We have recently designed a dedicated binary hierarchical data format to efficiently store,
organize and process ribosome profiling data.
We are building a computational ecosystem around this file format (<a href="https://academic.oup.com/bioinformatics/article/36/9/2929/5701654">.ribo</a>).
We currently have a workflow that can generate these files starting
from raw sequencing reads.
The resulting file can be used seamlessly to analyze and visualize
in our downstream analysis software. We continue to improve this ecosystem
by adding ribosome profiling specific analyses such as improved algorithms
for pause site detection. 

We emphasize development of reusable, portable and open source software that will be widely distributed.
