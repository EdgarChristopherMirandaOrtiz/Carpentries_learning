# Carpentries_learning
Where I'm learning carpentries 

## Project Organization and Management for Metagenomics

### Documents before sent DNA or RNA off for sequencing

- Spreadsheet od the data of our experimente (whatever we were measuring)
- Lab notebook
- The data of the samples
- How we're goint to sequence (DNA or RNA, pair-single-end, Illumina?, what we expect?)

### Creating a github space →  README file

- Date format for documents (dd,mm,yyyy)
- Meaning abbreviations
- Meaning or pattern of IDs samples
- Detailed methodology
- Information of authors
- Meaning and names of variables

### Ethical considerations → Microbiome

- Respect → Sign explicit prior informed consent
- Do good → Participant's privacy
- Do no harm → Policy of results communications
- Do no harm → Invasivness of sampling and minimize risks
- Act justly → Favor disversity of subjects and justice

### Structuring data in spreadsheet

- [1] Raw data remains as raw data
- [2] Observations in its on row
- [3] Variables in columns
- [4] use "_" instead of spaces
- [5] Separet info
- [6] CSV format
- [7] Fill with "0"
- [8] no tabs, no tabless
- [9] optimal file name

### Laaaaaaaarge data sets

They could use a lot of **disc space**, since we have the large data sets and its **pipelines** including intermediate and result files. As a resutls identifiying **errors is complex**. 

### Retrieving sample sequenceing data from Sequence Center

- Samples are organized by sample_ID
- The _R1 and _R2 mean Read1 and Read2, like for 5'-3' and 3'-5'
- **.gz** → means "gzip", that is compressed

### Storing dat

- Accesible at least for the head and others team member access
- Place redundantly backed up and in different locations
- Raw data reamins raw data

### Public data

Almost all analysis use **reference data**, and we may want to **compare our results** and **annotate** data in our sequences. 

When we want to publish a paer we surely will need to **public our sequencing data**. This sharing makes our **paper more likely to be re-used and cited**

- NCBI → National Center for Biotechnology Information
- ENA → European Nucleotide Archive (EMBL-EBL)
- SRA → Sequence Read Archive

### Accesing data (EXAMPLE)

**Paper name:** Genomic adaptations in information processing underpin trophic strategy in a whole-ecosystem nutrient enrichment experiment

**Doi:** https://doi.org/10.7554/eLife.49816

**Bioproject information/reference:**

<img width="697" height="389" alt="image" src="https://github.com/user-attachments/assets/c770a4d1-4313-4dbd-939f-7cf541a5caa2" />

- **[1]** Go to database center → NCBI
- **[2]** Search the "bioproject"
- **[3]** Go to "Project Data"
- **[4]** Clicl on the number of SRA experiments, this case is 40
- 
<img width="445" height="208" alt="image" src="https://github.com/user-attachments/assets/b0e890a0-60de-40c2-af16-30144763b065" />

- **[5]** Go to "SRA Run Selector" to see the collection of all the experimental data
- 
<img width="1918" height="1197" alt="image" src="https://github.com/user-attachments/assets/17536c91-7b4c-4ff9-b802-91eb355e774f" />
<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/0753d3c3-42d6-43cb-bfbe-a6f8c08511c2" />

- **[6]** See  “Common Fields”, “Select”, and “Found 40 Items”
- 
<img width="1918" height="1199" alt="image" src="https://github.com/user-attachments/assets/15c0bda1-8d08-4aaf-90e0-4f0ad8eacfa7" />

  -  **"Select"** contains information about the run size and the data and metadata table; there were 40 runs, 9.86 GBytes of data, and 19.61 Gbases.
  -  **“Found 40 items section”** is a table where each row contains id numbers, an alias name, size and links to data for one sample. Within “Found 40 Items”, click on the first Run number

- **[7]** Click on the first Run number (Column “Run”, Row “1”)

In the image we see the SRA entry ERR2143758. This metadata tab displays run’s quality and GC content among other information.

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/166d61ee-978e-48a1-a6ff-4b75201eadbb" />

- **[8]** Go back, and then clic on "Metadata"

button to download the file “SraRunTable.txt” and save it on your computer

<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/b22d36f7-a132-4aea-98a4-208779483dd3" />

- **[9]** Open the SraRunTable.txt file

Docuemnts usually are separated by commas or tabs, so they are named with the .csv (comma-separated values) and .tsv(tab-separated values) extensions, respectively. But since they are both plain text files, you can find them with the .txt extension

> [!CAUTION]
> **avoid saving any changes you might have made to this file**
>  keep raw things raw

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/2c3b8faf-4e56-4d10-bfa3-c1b6dbc1f8ab" />


# SHELL

## A shell is a computer program that allos you to control your computer using commands entered with a **keyboard**, insteas of controlling the graphical user interface (GUIs)

- Many bioinformatics tools can onnly be used through a command line interface, also could have extracapabilities
- The sheel makes it less boring →a Atuomate repetitive tasks ans leave of files
- Work less error-prone. Humans can make mistakes even by ten times of doing the same
- Large amount of cimputing power → Meaning using remote computers or cloud computing
- 











