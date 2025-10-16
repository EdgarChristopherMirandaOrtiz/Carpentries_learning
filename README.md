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

A shell is a computer program that allos you to control your computer using commands entered with a **keyboard**, insteas of controlling the graphical user interface (GUIs)

- Many bioinformatics tools can onnly be used through a command line interface, also could have extracapabilities
- The sheel makes it less boring →a Atuomate repetitive tasks ans leave of files
- Work less error-prone. Humans can make mistakes even by ten times of doing the same
- Large amount of cimputing power → Meaning using remote computers or cloud computing

      clear → literally clears the terminal from script, not lost any info

      PS1='\W\$ ' → Shows the ultimate directory. Here is home directory (~)

      $ → prompt wainting for input

      pwd → print working directory ¿Where are we?

      ls → listing, to know

<img width="412" height="136" alt="image" src="https://github.com/user-attachments/assets/9c9bc84c-b8f6-4968-802d-e911112065ad" />

    cd → change directory, followed by a directoy name
  
<img width="471" height="104" alt="image" src="https://github.com/user-attachments/assets/ce3c004c-4326-41ce-ac93-b9b925cd5e96" />

    -F → a flag "/" to see if it's a file or a folder (directory)

<img width="440" height="138" alt="image" src="https://github.com/user-attachments/assets/7b039576-7855-49b8-bccb-c585f98c16ed" />

    man ls → To see other funtions
    tab → the next page
    b → backwards
    q → quit

<img width="627" height="221" alt="image" src="https://github.com/user-attachments/assets/8c86fb0d-baa6-4ccd-87be-a5ee640dcce9" />

    ls -1 → to see more infor woth the list setnisire

<img width="545" height="271" alt="image" src="https://github.com/user-attachments/assets/6a6d5dbc-2d87-4abf-89a1-e92ad3014d32" />

### Untrimmed_fastq directory

<img width="503" height="154" alt="image" src="https://github.com/user-attachments/assets/1d2e79bc-b693-4117-81e9-7ac8ea333da4" />

<img width="1035" height="215" alt="image" src="https://github.com/user-attachments/assets/e7e45ae0-c6e6-47c7-85b5-d830d7264bae" />

File  TruSeq3-PE.fa and .fastq.gz (GZ is an archive file compressed)

### FASTQ 

Format for storing information about sequencing reads and their quality

    gunzip → to descompess the files so that we can look at the FastQ format

<img width="1176" height="197" alt="image" src="https://github.com/user-attachments/assets/ed6857f2-7a4b-48d0-9486-96c5daef9350" />

### Shortcut: Tab completion

    tab → The "tab" key as in the console is used to autocomplete de name

    **When we have 2 or more documents/directories with the same prefix, we're gonna obtain as a result XXX_R and by clicking other 2 "tab" "tab" the options will be displeid

<img width="659" height="126" alt="image" src="https://github.com/user-attachments/assets/59030507-a84a-47da-b934-3f4d26cf2e56" />

<img width="1590" height="134" alt="image" src="https://github.com/user-attachments/assets/61021d0d-e67f-455c-92b6-6f95bcf9df43" />

### Navigating files and Directions

    cd → doesn't recognise directories if it is not on the current directory or if it is level above the one we are

    cd .. → is the one that lets you go back

<img width="1711" height="266" alt="image" src="https://github.com/user-attachments/assets/9be970ca-e282-45ad-b166-5c92dd47d4b8" />

### Hiding directories

    cd <tab> <tab> → by clicking appears the list of item, even those who are hidden

<img width="1121" height="211" alt="image" src="https://github.com/user-attachments/assets/0ca25b10-0f30-499b-b1fd-16d8b3620ad8" />

    ls -a is another way to find the hidden directories

### Current permissions of a file

This is useful when we want ot protect our documents from delitionor overwriting

    ls -l → means "long for the ls command, its L not 1

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/0d558bb6-5f1f-4217-9f51-8496e00fca4d" />

<img width="504" height="96" alt="image" src="https://github.com/user-attachments/assets/e82bd1c3-c42f-4611-a4f0-c64ce9cdb6f5" />

# Working with files

    ls *.fastq → used to list all the ".fastq" terminal files
    la *R1.fastq → lists all the "*R1.fastq"

as we can see, all after * is what is searched
    
<img width="684" height="50" alt="image" src="https://github.com/user-attachments/assets/31931221-b8a7-4820-be04-539c6267aab2" />

### Other useful commands

    Ctrl C → cancel the command you are writing
    Ctrl R → reverse-search
    Ctrl L → clear the screen

### History commands

    history → the history of comands

    !271 → will call the command 271 of the history

<img width="654" height="273" alt="image" src="https://github.com/user-attachments/assets/49b98831-2e9e-4d74-8102-c9fdf6477904" />

# Examining files

    cat → used to read files, but it open it even if big
    Ctrl C → to stop

<img width="1749" height="318" alt="image" src="https://github.com/user-attachments/assets/02c7598b-643b-41d5-b124-6870b4c6d3e4" />

    less → will open the read mode
    
    Space → go forward
    b → go backward
    g → beginning
    G → end
    q → quit
    /[word] → search a specific word from the beginning of the document or forward
    ?[word] → search a specific word from the end of the document or backwards

<img width="1748" height="305" alt="image" src="https://github.com/user-attachments/assets/d9b87416-ccb3-42c0-93e9-419762b6c178" />

    head → beginning of a doc

<img width="1730" height="264" alt="image" src="https://github.com/user-attachments/assets/b5b0ea5c-5edd-4de2-8251-a48330ce8f31" />

    tail → end of a doc

<img width="1738" height="257" alt="image" src="https://github.com/user-attachments/assets/e8e42bff-e7c6-4310-bf9d-9477ce98559e" />

    -n # → shoes the first or last n lines of a file when "head" or "tail"
    
<img width="1730" height="102" alt="image" src="https://github.com/user-attachments/assets/a23d8e35-e4a7-4079-992c-2c878e8ac7ac" />

<img width="1723" height="126" alt="image" src="https://github.com/user-attachments/assets/5ebdc5ac-2e03-4eb2-ae30-68a74e7a27cd" />

### FastQ interpretation


**Line - Description**
- [1]	Always begins with ‘@’ and then information about the read
- [2]	The actual DNA sequence
- [3]	Always begins with a ‘+’ and sometimes the same info in line 1
- [4]	Has a string of characters which represent the quality scores; must have same number of characters as line 2

<img width="1723" height="137" alt="image" src="https://github.com/user-attachments/assets/c0040d07-12b6-4459-8276-41347fb74c74" />
This is actually a good read!

Line 4 shows the quality for each nucleotide in the read. Quality is interpreted as the probability of an incorrect base call

Each character is assigned a quality score between 0 and 42 as shown in the chart below.

<img width="486" height="97" alt="image" src="https://github.com/user-attachments/assets/b8ce6392-dee4-4a09-a273-561a86636a70" />
Each quality score represents the probability that the corresponding nucleotide call is incorrect.

This quality score is **logarithmically based**, so a quality score of 10 reflects a base call accuracy of 90%, but a quality score of 20 reflects a base call accuracy of 99%. 



### COPYING FILES

    cp [orignal name document] [name of the copy document] → gives the original document and the copied one 

<img width="1326" height="93" alt="image" src="https://github.com/user-attachments/assets/676f43aa-5ab0-4f3f-8245-1e3adabbff05" />


### CREATING DIRECTORIES

    mkdir [directory's name] → make a directory, do not add the "[]" jsjs

<img width="1444" height="69" alt="image" src="https://github.com/user-attachments/assets/076e8ad7-bfb9-4b75-8b7d-f0f5beab4985" />


### MOVING FILES

    mv [FIle name] [Directory where it'll be placed]

<img width="885" height="84" alt="image" src="https://github.com/user-attachments/assets/9d8f510a-dae6-4fdd-93fd-43a04e5d51a3" />


### RENAMING FILES

    mv [original name] [new name] → to change one file's name or directory's name

<img width="1071" height="118" alt="image" src="https://github.com/user-attachments/assets/4a2e70de-1fa4-4e17-854b-e8460d0e7d76" />

<img width="1218" height="149" alt="image" src="https://github.com/user-attachments/assets/15a26f57-c8b9-4472-887e-76e9ed1c6dff" />


### REMOVING FILES or DIRECTORIES

> [!CAUTION]
> **rm permanently removes, they're really gone**

    rm [file's name] → remove files
    rm -r [directory's name] → remove directory and all files withing it. If some write-protected files you'll be asked to overrride our permission

<img width="955" height="41" alt="image" src="https://github.com/user-attachments/assets/f4853a1d-a38f-4116-88ca-68e777ecc5a1" />

<img width="1171" height="108" alt="image" src="https://github.com/user-attachments/assets/7bb6d9e2-b829-42b9-80f6-4d403c56942a" />

<img width="772" height="169" alt="image" src="https://github.com/user-attachments/assets/1a92d641-3ea5-4759-abcd-f55d7c264799" />


# SEARCHING ON FILES

The four nucleotides that appear in DNA are abbreviated **A**, **C**, **T** and **G**
Unknown nucleotides are represented with the letter **N**

### Search 10 N's in our reads

    grep NNNNNNNNNN JC1A_R2.fastq → grep is to search on files without opening them 

This noisy, as grep returns a lot of output, every single line in the file that contained 10 N's
, regardless of how long-short the file is. Additionally it just shows the sequence but not the identifier

<img width="1722" height="223" alt="image" src="https://github.com/user-attachments/assets/7a765007-e52c-4234-8e35-e467ef4b3ddd" />

    grep -B1 -A2 NNNNNNNNNN JCA1_R1.fastq 
    -B → number of lines before each match
    -A → Specific number of lines after each matching line
    **BUT WE WANT A LINE BEFORE AND 2 AFTER THE MATCHING LINE, SO:
    -B1 -A2

<img width="1716" height="262" alt="image" src="https://github.com/user-attachments/assets/18a7892e-56cc-4dcc-87cc-d76f4728f2d6" />

<img width="1719" height="183" alt="image" src="https://github.com/user-attachments/assets/5410875e-45eb-46a5-b219-eb16d8f1d5fd" />


### Find a sequence in all documents

    grep -B1 AAGTT *.fastq

<img width="1736" height="268" alt="image" src="https://github.com/user-attachments/assets/652ea023-d82d-443a-8975-c0c92ea9505a" />

# Redirecting output

Here we need to capture the output obtained by grep, the sequence mathing on the documents I mean

Objective ► obtain the matching data and redirect it to another location/file as we'll want to analyze it later 

    grep -B1 -A1 [sequence] [original document] > [new location/file]
    grep -B1 -A2 NNNNNNNNNN JC1A_21.fastq > bad_reads.txt

<img width="1145" height="154" alt="image" src="https://github.com/user-attachments/assets/4e608a17-68d0-4a7d-a90d-5eb5e1717492" />

### See how many lines we have

    wc [file] → to see how many words, lines and characters are in the file

<img width="774" height="42" alt="image" src="https://github.com/user-attachments/assets/ce792db8-9070-49d2-b088-973b657f759d" />

    wc -l [file] → just to see the number of lines, again is "L" not "1"

<img width="781" height="93" alt="image" src="https://github.com/user-attachments/assets/11f2407c-c742-472e-9062-18cdc48e2c52" />

> [!CAUTION]
> Every time we want to add information on the file selected to use wc, we are overwriting on it; it means, that for example you have to files you met the first wc, then go to the second one, this seconf info will replace the first file info.

To avoid overwrinting use **>>** : 

    grep -B1 *A2 NNNNNNNNNN JC1A_R2.fastq >> bad_reads.txt
    wc -l bad_reads.txt

<img width="1100" height="211" alt="image" src="https://github.com/user-attachments/assets/c18e9913-d760-464d-8d73-3ddab6126150" />

### Matching lines by less

That is why grep can redirect to a new location (less) or file 

    grep -B1 -A2 NNNNNNNNNN JC1A_R2.fastq | less

<img width="1733" height="309" alt="image" src="https://github.com/user-attachments/assets/5117c0f8-32ad-44c2-9a9e-62df145286f0" />


# Writing LOOPS

for → is for repeat a command or a group o commands

Each time the loops run (an iteration), an item is assigned as the variable and commands are executed before moving into the next item

**$ → CALL THE VARIABLE**

The "$" symbol tells to the shell to treat the variable as a variable name and substitute its value in its place.

    for filename in *fastq → saying the variable (filename) indicating the whole universe of *fastq files
    do → literally "do"
    head -n 2 ${variable} >> [final document] → (-n 2, says taking the n head lines), (${variable}, treat the variable as a variable), and the outcome variable/file, (>>, add instead of overwrite)
    done → to close the for

- The variable could be designed in the moment of the loop

<img width="856" height="124" alt="image" src="https://github.com/user-attachments/assets/fef7733d-001b-45ba-aa73-f0a45170ef02" />

    cat → to see the loop made on the seq_infor file

<img width="1741" height="274" alt="image" src="https://github.com/user-attachments/assets/eb04a9c7-713f-44d8-9451-b182f938ede8" />

# BAsename FOR LOOPS

Is for removing a uniform part of a name from a list of files

    basename [file's name] [wanted part to be deleted] → to quit some part of file's name
    basename JC1A_R2.fastq .fastq

-  It work wtih EXACTLY matches

<img width="884" height="40" alt="image" src="https://github.com/user-attachments/assets/83207ff9-0c90-469b-8fec-a684647be540" />

    for filename in *.fastq → for [variable] in [universe]
    do
    name=$(basename ${filename} .fastq) → first delete .fastq in the variable (filename) in progress in that iteration, and store it into "name"
    echo ${name} → will print the variable "name" each time the loop runs
    done

- Para crear variables los espacios si importan, no dejes espacios entre el = 

<img width="1380" height="127" alt="image" src="https://github.com/user-attachments/assets/b54cca3d-1ec7-4173-bfb9-8e63b132e549" />

<img width="1253" height="215" alt="image" src="https://github.com/user-attachments/assets/5ea276d6-7e40-4652-8234-ea81d5cf2c88" />

### Rename in loop

    for filename in *.txt → (*#### is just to indacte witch math to search, not changing that prompt)
    do
    name=$(basename ${filename} .txt)
    mv ${filename} ${name}_2019.txt → here mv is used to rename as mv [originalname] [new name]
    done

<img width="1495" height="210" alt="image" src="https://github.com/user-attachments/assets/1ff8d0f1-c2eb-41c8-82c9-128c1eaa6702" />

<img width="1671" height="107" alt="image" src="https://github.com/user-attachments/assets/b4ef1546-49c8-4793-93d8-8c0eff3c69cc" />

As it just take the *.txt it means if we re-run the prompt the _2025 will be write again if we are correct, and of course it did it

<img width="1607" height="111" alt="image" src="https://github.com/user-attachments/assets/f3bf0cb0-2c4a-485b-9f5d-a2751f49fd1e" />

<img width="1721" height="272" alt="image" src="https://github.com/user-attachments/assets/2b910a93-c83f-4dd8-8c64-c091ffe2eed6" />


# WRITING FILES

NANO, to create a README.txt file, as where I'm writing right now

JUST **TEXT**, not tables, etc

    nano README.txt

The text in the bottom shows the shortcuts

<img width="1727" height="298" alt="image" src="https://github.com/user-attachments/assets/00804a00-41ea-4e6e-b53a-57cd6bf57d52" />

<img width="1746" height="335" alt="image" src="https://github.com/user-attachments/assets/eca04a10-4e4e-4de1-b825-766a3d225fb9" />

    Ctrl O → For opening
    Ctrl X → return to shell
    Ctril S → Save

### Matching and redirecting to file

    grep -B1 -A2 NNNNNNNNNN *.fastq > scripted_bad_reads.txt → here we saw for the matches with 10 N's and then added to a new file

<img width="1358" height="108" alt="image" src="https://github.com/user-attachments/assets/986c858f-7a37-49ea-b3b7-30974d7ec73c" />

### Adding the commands into a file

    nano bad_reads_script.sh → "sh" doesn't means anything but tell us it is a **shell script**

It opens a file to text, we also added the grep command to obtain the bad data

<img width="1735" height="341" alt="image" src="https://github.com/user-attachments/assets/bf09ef86-c67f-4529-a7da-e12026fe442b" />

    nano bad-reads-script.sh → this instructions just openned and creted the file

For now seems like nothing happened but if you open the file you made on the other text file you'll it worked (with nano [file name])

<img width="1755" height="335" alt="image" src="https://github.com/user-attachments/assets/7e2e69ee-1236-4e0f-af80-977a3e173fbf" />

<img width="1753" height="353" alt="image" src="https://github.com/user-attachments/assets/f9b2888a-ef56-4e56-ac60-fb1ea97563b0" />

To run the document:

    bash bad-reads-script.sh → this runs the script on our file
    Ctrl X → allows us to get out of the text file
    echo "Script finished!" → at the end echoXXX is printed

<img width="865" height="37" alt="image" src="https://github.com/user-attachments/assets/da0a9c07-85eb-4cc3-9cd1-bc17a644ae4e" />

# Script into a program
