---
title: "Cancer Informatics for Research Leaders"
output: html_document
---

# Introduction 

## Motivation
This course will cover the key cancer informatics topics principal investigators (PI) and other research leaders need to know when running a lab. 

**Target Audience:**  
The course is intended for PIs and other lab leaders who want to learn how to transition their labs to using cancer informatics tools, for those who rely on cancer informatics but for whom it is not a core competency, as well as, PIs for whom informatics is a key part of their research. 

**Curriculum:**  
This course will feature a range of ITCR tools from the very general (Galaxy7, Bioconductor56) to those that are very application specific (CRAVAT10, CIVIC13) but tools will only be featured at a conceptual level, rather than through hands on engagement in workflows. For more in-depth information about particular tools, see our other courses at our website: www.itcrtraining.org. 

The curriculum will also cover the roles and responsibilities of a lab leader in collaborative, mentor, or employer relationships with informatics experts. It will cover budgeting for cancer informatics locally or on the cloud, as well as key responsibilities for research leaders in data security, privacy, management and reproducibility.  


## Informatics for Cancer Research

Biomedical research at large, and in particular cancer research, now involves massive amounts of data of a variety of types collected through rapidly advancing technologies. To allow current and future cancer researchers to fully take advantage of the opportunities afforded by these technologies, our mission is to make informatics tools as accessible as possible to all cancer researchers.  From omics, to imaging, to clinical data, cancer researchers can now examine biospecimens, animal models, and clinical data with unprecedented depth and breadth.

This course aims to provide an overview of tools available to cancer researchers to afford them more flexibility in their research. It will also provide guidance for best practices for performing informatics research.


## Tools

### Galaxy

This section was written by Jeremy Goecks:

Galaxy is a web-based computational workbench that connects analysis tools, biomedical datasets, computing resources, a graphical user interface, and a programmatic API (Figure 1). Galaxy (https://galaxyproject.org/) enables accessible, reproducible, and collaborative biomedical data science by anyone regardless of their informatics expertise. There are more than 8,000 analysis tools and 200 visualizations integrated into Galaxy that can be used to process a wide variety of biomedical datasets. This includes tools for analyzing genomic, transcriptomic (RNA-seq), proteomic, metabolomic, microbiome, and imaging datasets, tool suites for single-cell omics and machine learning, and thousands of more tools. Galaxy’s graphical user interface can be used with only a web browser, and there is a programmatic API for performing scripted and automated analyses with Galaxy.

Galaxy is used daily by thousands of scientists across the world. A vibrant Galaxy community has deployed hundreds of Galaxy servers across the world, including more than 150 public and three large national/international servers in the United States, Europe, and Australia (https://usegalaxy.org, https://usegalaxy.eu, https://usegalaxy.org.au). The three national/international servers (Figure 2) have more than 250,000 registered users who execute >500,000 analysis jobs each month. Galaxy has been cited more than 10,000 times with >20% from papers related to cancer. The Galaxy Tool Shed (https://usegalaxy.org/toolshed) provides a central location where developers can upload tools and visualizations and users can search and install tools and visualizations into any Galaxy server. Galaxy has a large presence in the cancer research community. Galaxy serves as an integration and/or analysis platform for 7 projects in the NCI ITCR program. There is also increasing use of Galaxy in key NIH initiatives such as the NCI Cancer Moonshot Human Tumor Atlas Network (HTAN) and the NHGRI Data Commons, called the AnVIL (https://anvilproject.org/).

Galaxy’s user interface, accessible via a web browser, provides access to all Galaxy functionality. The main Galaxy interface (Figure 3) has three panels: available tools (left), running analyses and viewing data (middle), and a full history of tools run and datasets generated (right). Datasets for analysis in Galaxy can be uploaded from a laptop or desktop computer or obtained from public data repositories connected to Galaxy. With Galaxy, complex workflows composed of tens or even hundreds of analysis tools can be created and run. In Galaxy’s workflow interface (Figure 4), tools can be added and connected via a simple drag-and-drop approach. Galaxy users can share all their work—analysis histories, workflows, and visualizations—via simple URLs that are available to specific colleagues or a link that anyone can access. Galaxy’s user interface is highly scalable. Tens, hundreds, or even thousands of datasets can be grouped into collections and run in parallel using individual tools or multi-tool workflows. In summary, Galaxy is a popular computational workbench with tools and features for a wide variety of data analyses, and it has broad usage in cancer data analysis.


