# exploreSA-Gawler

> Background: This github project is part of the exploreSA competition on [unearthed.solution](https://unearthed.solutions/u/competitions/exploresa)  Here is [my original post](https://unearthed.solutions/u/competitions/80/forum#/question/441d6535-6d37-4550-88b9-12bc0c0a5342) on exploreSA forum to explain what our team has done for the data cleaning part. For more information please visit the unearth website there is [detailed description page](https://unearthed.solutions/u/competitions/exploresa) 

---

## Table of Contents

- [Description](#description)
- [How to use](#how-to-use)
- [To be continue](#to-be-continue)

### Description

**Drilling, surface sample and observations data: A dataset with features and labels**

The SARIG Data Package is an extract from the Geological Survey of South Australia’s (GSSA) geoscientific database SA Geodata. The data package includes a series of CSV files covering 4 parts:

*  Drill holes data, including the metadata of drill holes, and the geological, petrophysical, lithological data

* Field observation data, including general observation, lithological and geological structure data.

* Mineral deposits data, including location, lithology, mineralogy data

* Rock sample data, including biostratigraphy, geochronology and petrography analysis data

This dataset plays an important role in the whole data pool used for predicting the cores in Gawler area. Since the dataset includes the commodities information and the elements from the geochemistry analysis which suggest the occurrence of the minerals. In other words, the labels for the training dataset is defined. The attributes of these datasets can be cleaned as features in the following machine learning modelling.



### Installation and Packages

Step 1. Install Python 3.6 and use pip install packagenames to install the following packages:
 1. set up the jupyter notebook environment
 2. pandas
 3. zipfile
 
     or optionally, install Anaconda and use conda install packagenames

Step 2. run the ipynb files according to the filenames order:
     a) execute "1. RS_Data_Processing.ipynb" from the beginning until the dropdown box and the code will download the datafiles from the link: https://unearthed-exploresa.s3-ap-southeast-2.amazonaws.com/Unearthed_5_SARIG_Data_Package.zip if the zip file does not exist in the directory './data'
     b) select the element you are interested from the dropdown box, then continue to 'Run ALL Below'. The code will generate two csv files: 'rs_chem_site_sample_num.csv'and 'extracted_rs_data.csv' and save them to a subdirectory of './data', named after the element you selected; e.g., 'Fe'. The former includes the 'SITE_NO' and 'SAMPLE_NO' corresponding to the element you selected above, while the latter is the rs data related to this element.
     c) execute "2. Drillhole_Data_Processing.ipynb", "3. Field_Observation_Data_Processing.ipynb" and "4. MD_Data_Processing.ipynb" will generate the corresponding drillhole data, field observation data and mineral deposit data and save to directory corresponding to the element.      d) further merge the data files to get the work datasets.  

The idea of this repo is to show people the cleaning data process we have done until now. There are still a lot of work to do. We will keep updating the data preparation and our dat engineering results.



### To continue





 



