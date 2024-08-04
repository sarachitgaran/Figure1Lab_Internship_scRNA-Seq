---
Author: Sara Chitgaran
Date: 2024-07-22
---

# Figure1Lab-Internship-scRNA-Seq 📝

## Introduction

Welcome to my Figure1Lab internship repository. This project aims to help students hone their compbio skills by emulating an internship in biotech/pharma company. The goal is to determine the efficacy of anti cancer drugs by exploring single cell RNA-Seq data in cancer cell line.

This repository is dedicated to my progress of diving deep into the realm of scRNA-seq where I summarize papers I read and share codes as well as my own thoughts.

**Week1 Memo**

The first week of the internship is devoted to the literature review in order to learn the neccessary content that will be of use in the following weeks. I have to address the Key Scientific Questions (KSQ) and paraphrase it with my own words.


## Original Question

The original question provided for the first week's task is: **"Using available scRNA-seq data from cancer cell lines, how would you explore the use of the following FDA-approved antibody therapies in additional cancers??
 -Trastuzumab: Targets HER2 and is used in the treatment of HER2-positive breast and gastric cancers.
 -Bevacizumab: Targets VEGF and is used for a variety of cancers, including colorectal, lung, glioblastoma, breast, liver, and kidney cancer."**

### Literature Review

In order to break down the question into its buildig blocks, first we need to have a somewhat comprehensive literature review of the underlying biology and methodolgy of the question we have in mind.



__Cancer cell line__

Cancer Cell line Encyclopedia project was established in 2006 as a result of the collaboration between Braod Institute and Novartis Institute. It is like an equivalent of TCGA for cancer cell lines. So far, CCLE did a huge service to the filed of biology so far as it provided scientist with the genome-wide characterization of the cancer cell lines which can be corporated in different studies such as testing anticancer drugs and evalauting cell responces in a nearly controlled environment.  
Although cell lines are very good models (due to their affordability and availablity) to predict drug sensetivities of different cancer, they have their own drawbacks:

To start with, they may not capture everything as they may horbor genetic variations which may not be present in the cancer cell itself. These mutations usually occurs as a result of extensive passages in cell cultures and may play a role in the final responce to the drugs. Moreover, by isolating cells in a dish, we are deliberately divorcing those cells from the natural environment they were at. Therefore, they do not represent the whole complexity and heterogeneity of cancer as a result of being artificially maintained in the lab. With all that being said, they are still one of the best method for experimentalist to mimic the physiology and state of cancer cells in vitro in order to test the efficacy of anticancer drugs.

__Anticancer drugs__

Before jump into the world of anticancer drugs, let's take a breif look at cancer itself and try to answer some (seemingly!) basic questions about this mysterious diseas which have baffled scientists for centuries. 
 what is cancer and what are the characteristics of cancer cell?

Cancer is a complex disease and there are more than 220 types of cancer. All of them their own differences which make them unique in some way but the fundamental principle of all cancers is uncontrolled cell proliferation which result in tumors formation in the specific part of the body which may ultimatley results in metastasis to other organs. But what leads to this? We can refer to one of the key paper in cancer research to answer this question. Tumor cells take advantage of some molecular mechanisms inside the cell in order to bypass the regulatory framework embedded in the cell. According to Hanahan and Weinberg key paper in cell 2000, these are the 6 unique features of cancer cells:
 Evading apopptosis
 Self-sufficiency in growth signals
 Insesitivity to anti-growth signals
 Sustained angoigenesis
 Limitless replicatibe potential
 Tissue invasion & metastasis

What is the purpose of anticaner drugs? how they work? Whata re some example of anticancer treatment?

The overarching goal of anicancer drug is to eliminate cancer cells or at least slow down their growth. One kind of anticancer drugs are monoclonal antibodies which are labratory-made moleculae that can act as an stimulator for human immune system. As soon as they enter the body (they are injected through the vein) they provoke the immune system cells. They are considered targeted therapy as they can precisely aim and attack specific cancer cell.

__Vascular endothelial growth factor (VEGF)__ is a signaling protein which can act as a growth factor for vascular endothelian cells. This angiogenic factor is up-regulated in different types of cancer due to its role in neovascularization. One strategy to battle cancer is to use anti-VEGF to prevent VEGF from angiogensis. By depriving cancer cells from blood supply, the tumor is starved to death. __Bevacizumab__ is a drug treatment which can target VEGF, hence slowing sown the tumorigensis.


__Human Epidermal Growth Factor Receptor 2 (HER2)__ is also another protien involved in cell growth and __Trastuzumab__ (aka Herceptin) is a monoclonal antibody which kill tumor cells by targeting the HER2 attached cancer cells. Obviously it only works on HER2 positive cancers.



__scRNA-seq__


RNA sequencing provides us with a snapshot of molecular dynamcis inside the cell, tissue or organism at one specific timepoint. The data obtained through this method can be used to compare various samples and detect changes in different states, whether a disease, a new treatment or even different stages of development. Sequencing of RNA can be carried out in 2 ways: 1) Bulk RNA-seq: Sequencing the mixed RNA from the desired sample. 2) Single cell RNA-seq: Sequencing the transcriptome of individual cells which produce loads of valuable information and therefore it is more expensive and complicated. In order to draw biologically meaningful conclusions from scRNA-seq data, we need to acquaint ourselves with the piplines and softwares available for data analysis which are mainly writtem in python and R.

The result of bulk RNA-seq is the cell average expression profile which is easy to interpret and analyze. However, it does not reveal the true complexity at the molecular level and may hide some important information such as gene expression hetergeneity. Moreover, some drugs may only affect a specific type of cell which is only detectable with the increased resolution that only scRNA-seq offers.

There are 3 general steps to sequence RNA in either of these technologies: 1) Sample and library preparation 2) Amplification and Sequencing 3) Data output and analysis.
Currenlty for 3 kind of scRNA-seq protocols for the library preparation step exist, which are categorizaed mainlt base on the cell isolation protocol:
I. Microfluidic device-base strategies which  use hydrogel droplets to encapsulate cells.
II. Well plate base where cells are physically seperated into wells.
III. Fluidigim C1 which is a commercial chip that loads and isolate cells into small reaction chamber.

Each of these methods come with their own pros and cons and scientists should be aware of their biases when analysing the data. They are different in many aspects such as their ability for transcript recovery or number of sequenced cells and so on. Selecting either of them depends on the aim of the study. For example, droplet based assay are known outcompete other methods for capturing heteregeneous mixture of cells and therefore result in broader characterization of the 



__References__

- [Single cell best practice book](https://www.sc-best-practices.org/preamble.html)
- [Types of cancer (Cancer Research UK)](https://www.cancerresearchuk.org/about-cancer/what-is-cancer/how-cancer-starts/types-of-cancer#:~:text=For%20example%2C%20nerves%20and%20muscles,breast%20cancer%20or%20lung%20cancer.)
- [The hallmarks of cancer] (https://pubmed.ncbi.nlm.nih.gov/10647931/)
- [Cancer Cell Line Encyclopedia](https://sites.broadinstitute.org/ccle/#:~:text=Cancer%20cell%20lines%20are%20the,and%20for%20defining%20drug%20efficacy.)
- [Advantages And Disadvantages Of Using Primary Cells In Cell Culture](https://www.kosheeka.com/advantages-and-disadvantages-of-using-primary-cells-in-cell-culture/#:~:text=Continuous%20types%20of%20cell%20lines,in%20case%20of%20extensive%20passaging.)
- [Monoclonal Antibodies(Cleavland Clinic)](https://my.clevelandclinic.org/health/treatments/22246-monoclonal-antibodies)
- [What is VEGF](https://www.news-medical.net/life-sciences/What-is-VEGF.aspx)
- [VEGF and its role in non-epithelial cell](https://www.ncbi.nlm.nih.gov/books/NBK6482/)
- [Trastuyumab (Cancer Research UK)](https://www.cancerresearchuk.org/about-cancer/treatment/drugs/trastuzumab#:~:text=Trastuzumab%20is%20a%20type%20of,factor%20receptor%202%20(HER2))



----------
**Week2 Memo**

The main focus of the second week was to understand kinker paper and try to answer some questions mentioned below. Here are my thoughts to address the questions Dean lee raised:

    1-How did the authors handle the potential caveat of co-culturing cell lines before profiling by scRNA-seq? Why do you think that caveat was or was not adequately addressed?
 
 In my POV, one of the drawbacks of culturing different cell lines next to each other (a.k.a co-culture) in the same petri dish is the interaction they may have with each other in the environment which would not be existed if they were cultured in seperate dishes (monoculture). These interaction whether be communication or even competition for common resources would result in altered gene expression in cell lines compared to normal consition. Therefore, this new molecular interplay  may lead to the emergence of new properties in cell lines including drug resistency or metastasis.
Although authors mentioned that the cell lines being co-cultured has relatively similar proliferation rate, I still doubt that 2 different cell lines could have such a synchronized cell state which could be considered exactly the same. As a result, I believe that the state of cell cycle that each cell lines were in during the experiment were slightly different and since cell state highly affect the dynamic of gene expression, it may cuase some unwanted heteregeneity in that regard. However, they somehow addressed this problem by clustering based on cell state.
 Moreover, they co-cultured the cell lines 3 day prior to transcriptome profiling which is a suitable time for mutation to occur in order to adapt cells to their new enviornment. These mutation may get fixed in some population and heavily affect the pattern of gene expression in that specific pool. However, they tackle this hypothesis by comparing the hetergeneity within cell line to intra cell line heterogeneity and found that there were not any significant difference. In addition, they conducted a control experiment where 6 specific cell lines were profiled with and without co-culturing for 3 days and realized that it has a modest effect in the average gene expression. They also observed that the heteregenity pattern were highly consistent between the two conditions.

    2-The authors identified discrete subpopulations of cells within a subset of individual cell lines (Fig. 2A-B). What might be the reason why some cell lines have these discrete subpopulations while others do not?

In this study minority of cell lines (11%) showed discrete clusters of cells based on variability of their expression pattern measured by NMF followed by density-based clustering (DBSCAN). I can speculate that the divergence observed in gene expression can arise from so many factors including the inherent difference in genetic background, epigenetic or evironment.



    3-What are Recurrent Heterogeneous Programs (RHPs) and how were they defined?
    
RHPs are defined as patterns of gene activity that are consistently observed re peatedly across different cell lines while varying in the details of their expression and can be associated to a specific biological process
In this paper, to make the comparison easier, instead of considering individual genes, they defined expression programs (consisted of some hundred co-expressed genes) and found low similarities between them, both within cell lines of the same cancer type as well as across different type of cancer, showing that discrete subpopulation tends to be unique and cell line-specific.
They also implemented NMF to each cell line in order to identify continuous cell state variablity.
    
    4-How do they identified RHPs related to in vivo programs of heterogeneity in tumors, and what evidence supports this relationship?
    
Out of 10 RHPs, 7 were similar to in vivo program indicated by highly significant overlap of important genes and high correlation of cell score. They further investigated this similarity in melanoma and HNSCC by a combined analysis of cells from cell lines and tumors to support the evidence.
    
    5-Where can you download the scRNA-seq data as shown in Figure 1B?
    
This is the direct link to download all the data realted to this paper at once:
https://singlecell.broadinstitute.org/single_cell/study/SCP542/pan-cancer-cell-line-heterogeneity#/
