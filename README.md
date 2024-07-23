# Figure1Lab-Internship-scRNA-Seq 📝

## Introduction

Welcome to my Figure1Lab internship repository. This project aims to help students hone their compbio skills by emulating an internship in biotech/pharma company. The goal is to determine the efficacy of anti cancer drugs by exploring single cell RNA-Seq data in cancer cell line.

This repository is dedicated to my progress of diving deep into the realm of scRNA-seq where I summarize papers I read and share codes as well as my own thoughts.

**Week1 Memo**

The first week of the internship is devoted to the literature review in order to learn the neccessary content that will be of use in the following weeks. I have to address the Key Scientific Questions (KSQ) and paraphrase it with my own words.


## Original Question

The original question provided for the first week's task is: **"Using available scRNA-seq data from cancer cell lines, how would you explore the use of the following FDA-approved antibody therapies in additional cancers??
 +Trastuzumab: Targets HER2 and is used in the treatment of HER2-positive breast and gastric cancers.
 +Bevacizumab: Targets VEGF and is used for a variety of cancers, including colorectal, lung, glioblastoma, breast, liver, and kidney cancer."**

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


__Human Epidermal Growth Factor Receptor 2 (HER2)__ is also another protien involved in cell growth. And __Trastuzumab__ (aka Herceptin) is a monoclonal antibody which kill tumor cells by targeting the HER2 attached cancer cells. Obviously it only works on HER2 positive cancers.



__scRNA-seq__

scRNA-seq vs. bulk RNA-seq
One of the famous analogy for comparing these 2 methods is the smoothie



__References__

- [single cell best practice book](https://www.sc-best-practices.org/preamble.html)
- [Cancer Research UK](https://www.cancerresearchuk.org/about-cancer/what-is-cancer/how-cancer-starts/types-of-cancer#:~:text=For%20example%2C%20nerves%20and%20muscles,breast%20cancer%20or%20lung%20cancer.)
- [Cancer Cell Line Encyclopedia](https://sites.broadinstitute.org/ccle/#:~:text=Cancer%20cell%20lines%20are%20the,and%20for%20defining%20drug%20efficacy.)
- (https://www.kosheeka.com/advantages-and-disadvantages-of-using-primary-cells-in-cell-culture/#:~:text=Continuous%20types%20of%20cell%20lines,in%20case%20of%20extensive%20passaging.)
- The hallmarks of cancer (https://pubmed.ncbi.nlm.nih.gov/10647931/)
- (https://my.clevelandclinic.org/health/treatments/22246-monoclonal-antibodies)
- (https://www.news-medical.net/life-sciences/What-is-VEGF.aspx)
- (https://www.ncbi.nlm.nih.gov/books/NBK6482/)
- (https://www.cancerresearchuk.org/about-cancer/treatment/drugs/trastuzumab#:~:text=Trastuzumab%20is%20a%20type%20of,factor%20receptor%202%20(HER2))

