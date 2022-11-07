---
layout: default
title: Hudson
parent: Projects
nav_order: 1
---

Over the past 6 months I worked a visiting researcher at the New York Genome Center where I co-developed a computational pipeline for spatial analysis of highly multiplexed images. I really recommend having a quick look at the poster I made of Hudson for annuil. 


The package documentation can be found here (In Progress)




#Overview/Abstract

Multiplexed imaging technologies are amongst the fastest growing areas of multi-omics. These technologies capture many parameters of single cells while preserving their spatial location. As such, there is a need for a flexible, robust, and easily deployed end to end computational pipeline for processing and analysis of the data such technologies produce. The goal of such a pipeline is to capture cell-type compositions in a localized shape-preserving manner. To help researchers achieve this goal, we have developed Hudson. It is a fully automated computational pipeline for spatial analysis of multiplexed images obtained primarily via PySeq2500, which is an open-source toolkit for repurposing the HiSeq2500 sequencing system as a versatile fluidics and imaging platform. Hudson preprocesses and segments the multiplexed image to identify micro-environments within the tissue section and performs spatial analysis upon the computed micro-environments. Hudson uses the Snakemake workflow management system and can be scaled up from a personal computer to a research computing cluster for heavy workloads. The pipeline begins with the essential pre-processing of the image. This includes background correction, registering channels, stitching the image tiles together, and removing overlapping regions. As part of preprocessing, Hudson deploys the PICASOnn algorithm to perform unmixing of signals from dyes with overlapping emission spectra. Once pre-processing is complete, the spatial analysis phase begins with instance segmentation to detect image labels and computation of mean intensity per label. The mean intensities for all available markers in each label are then used for cell type identification via clustering and comparison with a reference single cell sequencing dataset. The cell type identifiers and other image properties including the labels and label centroids are output as an Anndata object. Finally, Hudson extracts data from the Anndata object to build local spatial environments, compute relevant spatial statistics, and build a cell connectivity graph for researchers to use in their own downstream analysis. Importantly, the end result is consistent with the input data regardless of the underlying system architecture on which Hudson is deployed. Given the computationally intense and programmatically advanced nature of analyzing highly multiplexed images, Hudson saves significant time for researchers wanting to incorporate spatial information and serves the overarching goal of making spatial analysis more accessible.





![Image](IMG_9011.jpg){:height="50%" width="50%"}