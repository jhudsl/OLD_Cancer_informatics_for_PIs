---
title: "03-Informatics-tools"
output: html_document
---


# Informatics tools for Cancer Research

Biomedical research at large, and in particular cancer research, now involves massive amounts of data of a variety of types collected through rapidly advancing technologies. To allow current and future cancer researchers to fully take advantage of the opportunities afforded by these technologies, our mission is to make informatics tools as accessible as possible to all cancer researchers.  From omics, to imaging, to clinical data, cancer researchers can now examine biospecimens, animal models, and clinical data with unprecedented depth and breadth.

This course aims to provide an overview of tools available to cancer researchers to afford them more flexibility in their research. It will also provide guidance for best practices for performing informatics research.

For a brief introduction about different imaging methods see [here](https://www.independentimaging.com/abcs-imaging-difference-xray-ultrasound-mri-ct-scan/) and [here](https://www.radiologyinfo.org/en/info.cfm?pg=pet).

## ITCR Tools
On the [ITCR website](https://itcr.cancer.gov/informatics-tools), you will find a list of tools developed by researchers funded by ITCR. 

There are 5 general categories of tools.

1) Imaging Tools

From tools to segment PET-CT and MRI scans, to algorithms for assessing tumor heterogeneity based on immunofluorescence images of tissue slides, to repositories of radiology and pathology images, the ITCR Imaging tools offer a variety of support for image processing and image analysis. 

2) Omics Tools



3) Clinical

4) Data standards

5) Network Biology


## Imaging tools 

### Tools for slide image analysis

[Thrive](https://www.csb.pitt.edu/ith/) is a very comprehensive interactive GUI-based tool that appears well suited for users of all computationally experience levels and  in particular for users who wish to try a variety of algorithms for image processing for assessing tumor heterogeneity/diversity, as well as performing cell segmentation and cell quantification.

![](images/thrive1.png)

[[Source](https://www.csb.pitt.edu/ith/)]


![](images/thrive2.png)

[[Source](https://www.csb.pitt.edu/ith/)]

Another tool being developed is called the [Pathology Image Informatics Platform (PIIP)](http://pathiip.org/) that will be a similar all-in-one platform for viewing, annotating, sharing and managing whole slide images. There are plans to further develop the platform to interface with third party algorithms for segmentation, color normalization, biomarker quantification, and radiology-pathology fusion. This platform will use the Pathcore [Sedeen slide viewer](https://pathcore.com/sedeen/).


For more specific tools check out:

The Pathcore [Sedeen slide viewer](https://pathcore.com/sedeen/), which allows for color correction, pseudo-coloring, cropping, resizing, overlays of additional layers, registration, markup, and annotation. It currently supports Aperio SVS, Leica SCN, other TIFF-based formats, and JPEG-2000 images. Users can even create their own tools.

https://youtu.be/K34Gqt1ItYs

The [Quantitative Imaging in Pathology (QUIP)](https://sbu-bmi.github.io/quip_distro/) is a web-based tool that allows for interactive analysis, exploration, and management of whole slide tissue images. It also allows for users to create plots based on image features using FeatureScape. (requires docker and git)


https://youtu.be/dK4c6ti1Dvc

[HistoQC](https://github.com/choosehappy/HistoQC) - is an open-source tool written in python for examining slides for artifacts and computing slide characteristics (stain intensity etc.) for quality control and data standardization that uses [OpenSlide](https://openslide.org/demo/) for viewing slides.


### Tools for radiology image analysis

There are a variety of tools available to assist with analyzing computed tomography (CT) scans, Magnetic Resonance Imaging (MRI), Positron Emission tomogoraphy (PET) and other nuclear medicine scans, as well as Ultra Sound (US). 


#### [3Dslicer](https://www.slicer.org/) 

3D slicer is a powerful tool for CT, MRI, and US analysis, as well as microscopy analysis. This tool allows for interactive 3D visualization (volume rendering), and image processing including registration and segmentation. 
 
 ![](images/3Dslicer_intro.png)

[[source](https://slicer.readthedocs.io/en/latest/user_guide/getting_started.html)]

There are many additional 3D slicer extension tools such as:

- [PET-CT-CoSeg](https://github.com/IOWA-PETCT-COSEG/PETCT_Slicer_Extension) is a PET-CT co-segmentation extension of 3D Slicer.
- [many additional PET 3D slicer extensions](http://qin.iibi.uiowa.edu/) for normalization, segmentation, extraction of quantitative indices, and automating liver uptake measurements.
-  [SlicerDMRI](http://dmri.slicer.org/) performs additional diffusion MRI iamge analyses including command line batch processing, computing scalar maps, and registering multimodal data. It supports both DICOM and nnrd and nhdr images.



### Tools for medical image standardization
 
[dcmqi (DICOM - digital imaging and communications in medicine (dcm) for Quantitative Imaging (qi))](https://qiicr.gitbook.io/dcmqi-guide/) This platform provides libraries and command line tools for standardizing communication of quantitative image analysis using the DICOM standard. This is required for sharing data in some archives like TCIA. See [this article](https://doi.org/10.7717/peerj.2057) and [this article](https://doi.org/10.1177/0962280214537333) for more information. 
 
 




[Open Health Imaging Foundation (OHIF) medical imaging viewer](https://github.com/OHIF/Viewers) (replacing lesion tracker) - web application for viewing, annotating, and reporting on DICOM images in 2D and 3D.

[ePAD](https://epad.stanford.edu/) A radiology and tissue imaging analysis platform that supports analysis of tumor burden over time. See [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3998692/) for more information.


### Imaging archives and repositories:
12) TCIA - radiology and pathology images with annotations and clinical information and in some cases paired omics data
tools here too?
13) CDSA - pathology data from the Cancer Genome Atlas

### Specialized imaging tools:
14) Breast Radiodensity assessment
15) TOPAS - ionizing radiation imaging and therapy simulations
16) [Ivy Glioblastoma Atlas Project (Ivy GAP)](https://glioblastoma.alleninstitute.org/ish/) data and tools - Glioblastoma patient data including(MRI/CT scan data, as well as gene expression and anatomic characterization (ex. infiltrating vs cellular) of Glioblastoma tumor in situ hybridization (ISH) tissue sections and adjacent hematoxylin and eosin (H&E)-stained sections. See [the Ivy GAP database ](http://ivygap.org/) and [ivygapSE](https://github.com/vjcitn/ivygapSE) a tool that provides support for Summarized Experiment data - compatible for analysis in R for the tumor anitomical and gene expression data. See also [ivyGlimpse](https://itcr.cancer.gov/informatics-tools/ivyglimpse) to explore tumor image data and how it relates to survival and gene expression. See [this article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6414061/) and [this article](https://aapm.onlinelibrary.wiley.com/doi/abs/10.1002/mp.14556) for more information.

> "...an anatomically-based transcriptional atlas of human glioblastoma that aligns individual histologic features with genomic and gene expression patterns, thus assigning a molecular significance to the most important morphologic hallmarks of glioblastoma."

>To create the atlas, we surveyed the anatomic features by in situ hybridization (ISH), analyzed their transcriptomes by laser microdissection (LMD) and RNA sequencing (RNA-Seq), and validated the feature specific, gene expression enrichment of newly-identified markers by ISH (Fig. 1). We created a clinical and genomic database (http://ivygap.org/) for the 41-patient cohort (table S1) whose tumors (n=42) were evaluated to create the atlas. We describe gene sets whose expression is enriched in the anatomic features, measurements of intra- and inter-tumor heterogeneity, and a molecular subtype classification of transcriptomic samples from our atlas and The Cancer Genome Atlas (TCGA). Together, these two on line resources constitute the Ivy Glioblastoma Atlas Project (Ivy GAP).

20) Cancer Imaging Phenomics Toolkit (CaPTk) - GUI or command line. web portal with tools for imaging and phenomics analysis for clinical decisions - currently focused on brain, breast, and lung cancer. In addition to image analysis tools for registration, segmentation, and feature extraction, it also aid daignostics with prognostic modeling, risk etimation and radiogenomics. See [this article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7402244/) for more information. Designed for research purposes only and has not been reviewed or approved by the Food and Drug Administration or by any other agency. It is not intended or recommended for clinical applications.
https://youtu.be/WrjoJOxq4i8

![](images/CaPTK.png)
[[Source](https://cbica.github.io/CaPTk/index.html)]

21) RADIOMICS.io - radiographic phenotyping tool using automated algorithms - allows for users to engineer features or to perform data driven analyses. See [here](https://www.radiomics.io/science.html) for publications about using automated phenotyping using imaging. 

![](images/radiomics.png)
[[Source](https://www.nature.com/articles/ncomms5006)]



Data transfer/sharing/management:
17) Globus is similar to Xsede seems like... as is codalab

Imaging analysis platforms:
18) cbibop - no updates since 2015??? think we should just show [codaLab Project](https://codalab.org/) - open-source web-based platform that enables researchers, developers, and data scientists to collaborate, with the goal of advancing research fields where machine learning and advanced computation is used. https://youtu.be/WwFGfgf3-5s 
experiment management system and easy collaboration system  - includes competitions such as Liver tumor segmentation challenge

19) [XNAT](https://www.xnat.org/about/) - PET/CT (maybe MRI, MEG and EEG - look at connectomeDB???) data analysis
- upload DICOM data , organize and share data, view, query, and download data, perform analysis through a secure API with access to high-powered computing clusters



22) Region Templates...
23) [DCMTK](https://support.dcmtk.org/redmine/projects/dcmtk) - A set of command line tools for working with DICOM data, including examining and converting DICOM image files and data transfer and storage of images

### Galaxy

This section was written by Jeremy Goecks:

Galaxy is a web-based computational workbench that connects analysis tools, biomedical datasets, computing resources, a graphical user interface, and a programmatic API (Figure 1). Galaxy (https://galaxyproject.org/) enables accessible, reproducible, and collaborative biomedical data science by anyone regardless of their informatics expertise. There are more than 8,000 analysis tools and 200 visualizations integrated into Galaxy that can be used to process a wide variety of biomedical datasets. This includes tools for analyzing genomic, transcriptomic (RNA-seq), proteomic, metabolomic, microbiome, and imaging datasets, tool suites for single-cell omics and machine learning, and thousands of more tools. Galaxy’s graphical user interface can be used with only a web browser, and there is a programmatic API for performing scripted and automated analyses with Galaxy.

Galaxy is used daily by thousands of scientists across the world. A vibrant Galaxy community has deployed hundreds of Galaxy servers across the world, including more than 150 public and three large national/international servers in the United States, Europe, and Australia (https://usegalaxy.org, https://usegalaxy.eu, https://usegalaxy.org.au). The three national/international servers (Figure 2) have more than 250,000 registered users who execute >500,000 analysis jobs each month. Galaxy has been cited more than 10,000 times with >20% from papers related to cancer. The Galaxy Tool Shed (https://usegalaxy.org/toolshed) provides a central location where developers can upload tools and visualizations and users can search and install tools and visualizations into any Galaxy server. Galaxy has a large presence in the cancer research community. Galaxy serves as an integration and/or analysis platform for 7 projects in the NCI ITCR program. There is also increasing use of Galaxy in key NIH initiatives such as the NCI Cancer Moonshot Human Tumor Atlas Network (HTAN) and the NHGRI Data Commons, called the AnVIL (https://anvilproject.org/).

Galaxy’s user interface, accessible via a web browser, provides access to all Galaxy functionality. The main Galaxy interface (Figure 3) has three panels: available tools (left), running analyses and viewing data (middle), and a full history of tools run and datasets generated (right). Datasets for analysis in Galaxy can be uploaded from a laptop or desktop computer or obtained from public data repositories connected to Galaxy. With Galaxy, complex workflows composed of tens or even hundreds of analysis tools can be created and run. In Galaxy’s workflow interface (Figure 4), tools can be added and connected via a simple drag-and-drop approach. Galaxy users can share all their work—analysis histories, workflows, and visualizations—via simple URLs that are available to specific colleagues or a link that anyone can access. Galaxy’s user interface is highly scalable. Tens, hundreds, or even thousands of datasets can be grouped into collections and run in parallel using individual tools or multi-tool workflows. In summary, Galaxy is a popular computational workbench with tools and features for a wide variety of data analyses, and it has broad usage in cancer data analysis.


