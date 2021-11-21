---
title: "Develop Pipeline for Processing Flow Cytometry Data"
---

The client, Precision for Medicine, asked us to develop a R pipeline for processing flow cytometry data.

We reviewed data and pipeline requirements and created implementation plan. We implemented the pipeline using publicly available data and following guidelines from opencyto.org. We implemented gating pipeline for HVTN080. We performed autogating of raw FCS files with OpenCyto. We output gated data from the autogating pipeline. We visualized gated data using OpenCyto functions and wrote wrapper functions to increase flexibility in plotting options. We output patient level data by biomarker for downstream processing. And we documented the implementation steps.

Our pipeline was integrated into the client's service platform that powers their business.