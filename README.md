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

lets look at the permissions

    ls -l bad-reads-script.sh

<img width="809" height="83" alt="image" src="https://github.com/user-attachments/assets/49d7ca9d-e5e5-406f-a99f-a89e79102212" />

### Change file permissions

    chmod u=rwx,g=rwx,o=r+x bad-reads-script.sh

<img width="1016" height="84" alt="image" src="https://github.com/user-attachments/assets/c5dbb5bd-0774-4ad3-8784-5f739ae4049f" />

X is ssaying that we can run it as a program

<img width="539" height="202" alt="image" src="https://github.com/user-attachments/assets/f09876f9-f0ca-4838-9627-24aec5732a0d" />

<img width="749" height="512" alt="image" src="https://github.com/user-attachments/assets/d29bb4ef-8517-49eb-99f7-f30f102e98ec" />

### Run the script on the file

    ./bad-reads-script.sh → "./" is like saying "look here in the directory for the program"

<img width="764" height="41" alt="image" src="https://github.com/user-attachments/assets/acbc009e-1eec-41a4-9368-d51f9ba8ca8f" />

### Compress files

    gzip ~/dc_workshop/data/untrimmed_fastq/*.fastq 
    ls -lh ~/dc_workshop/data/untrimmed_fastq/*.fastq.gz → list of all comrpressed files

<img width="1115" height="110" alt="image" src="https://github.com/user-attachments/assets/0d983b9a-160d-4a56-9f24-ce61e463c79b" />

# DATA

### Gettting data

We have two main options/programs:

- wget → is the short form of "world wide web get”, and its basic function is to **download**
- cURL → “see URL”, so its primary function is to **display webpages or data** at a web address

      which [program] → It search on our downloaded programs, if we dont have it, it doesn't whoe anything

<img width="412" height="121" alt="image" src="https://github.com/user-attachments/assets/441a4867-678c-42e4-aa1f-c26c9ec4a99f" />

### Download

    wget [link]

<img width="1322" height="267" alt="image" src="https://github.com/user-attachments/assets/9e82b78b-89a5-41d7-92fb-5fab25d99f36" />

    curl -0 [link] → CAUTION!! it displays all the infor inside the link

"-0" flag → Is telling to download and save the file with the same name it had on server

<img width="1756" height="367" alt="image" src="https://github.com/user-attachments/assets/0731540d-6f2e-49be-b66a-2d050907445d" />

### Moving files computer-instance

Upload

    scp [file name to upload] [direction where it is on computer]
    scp local_file.txt dcuser@ip.address:/home/dcuser/

Download 

    csp [direction and file's name on instance] [direction where we want it to be downloaded]

# ORGANIZATION

**IS ESSENTIIAL**

It is often overlooked (pasar por alto) amidst (en medio de) the exciment of getting a fisrt lok at the new data.

For now we consider *BASIC*:

- Design of the sequencing experiment
- Biologic question
- Appropiate samples
- Enough statistical power to answer

# Creating THE DIRECTORIES

    cd
    pwd
    mkdir workshop
    mkdir workshop/docs
    mkdir workshop/data
    mkdir workshop/results

<img width="490" height="245" alt="image" src="https://github.com/user-attachments/assets/25b0d04b-a51e-4aa1-be24-c46ac0b477a3" />

    ls -R shows the contect in each sub-directories

<img width="667" height="200" alt="image" src="https://github.com/user-attachments/assets/3787743a-ec78-4f01-9fa5-796835913874" />

> [!CAUTION]
> **ALWAYS** save a copy of the raw data, a file(s) you never modified

Separtate data from result files

Data → New data, obtained, not results but input
Results → New documents generated, as output, by the terminal, etc.
DoCs → written analysis, thought about the eventual publication, notes, etc.

### Redirecting/copying history-protocol

    history | tail -n 10 >> workshop_log_2025_10_2025.sh → we take the final 10 instructions (| tail -n 10) we put on history and redirected them to a new file (>> XXX)

<img width="905" height="24" alt="image" src="https://github.com/user-attachments/assets/17aac6d0-2ff6-44d4-94a2-89962c3da1df" />

<img width="850" height="241" alt="image" src="https://github.com/user-attachments/assets/def6a60d-4f38-4ea0-bb59-66d692d8132a" />

### Editing history documents with nano

    nano [file document on .txt or .sh format]
    nano [workshop_log_2025_10_2025.sh]

<img width="1746" height="301" alt="image" src="https://github.com/user-attachments/assets/232562cc-b1e8-414c-a184-5c4e4cfb48cb" />

Here I will remove "history line" number 474, add comments

    Ctrl A → move to beginning
    Ctrl E → move to end

<img width="1731" height="366" alt="image" src="https://github.com/user-attachments/assets/926d675d-124d-4294-a6e5-d2e6d65725f6" />

- As it is redundant or not necessary to show all history, be sure to specify on your bitacora the main protocol, is means, just leave the important:

<img width="1748" height="376" alt="image" src="https://github.com/user-attachments/assets/b44eda3a-f42e-4125-a67d-43d3f49aab1f" />

> [!CAUTION]
> Mantain your bitacora out of the archives and subdirectories
> I mean, if you delete a directorie It'll be useful as the protocols were in the main home and weren't errased

### Move files backwards in directories

Here "." means move the final file/directory en the "location I am standing"

    mv workshop/docs/workshop_log_2025_10_06.sh .

<img width="1056" height="87" alt="image" src="https://github.com/user-attachments/assets/0fab43ea-db3c-4ad3-9db1-05516df59ae2" />


# R STUDIO

<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/e8217974-6eab-4225-a868-9cab3b965d9b" />

### DATA STRUCTURE

Differenct ways of recognizing data in R called data structure

### Vector

Sequence of data of the same type

    vec <- c("a", "b", "c")
    typeof(vec) % To see which type of data is the one loaded in the "vec" vector

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/f69bc3a5-9bb5-4ae6-b829-15eadfdd04f0" />

### Factor

Hols the names of categories "levels" and a set of the data in those categories

     fac <- as.factor(vec)
     fac

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/b036dfdc-221d-49a9-952d-841b44f50919" />

# METAGENOMICS

Are collections of genomic sequences from various (micro)organisms that coexist in a given space

They are *snapshots* that shows us part of the taxonomic and even metabolic or functional composition.

Since they are a ***mixture of sequences***:

- What species are represented in the smaple?
- What are they capable to do?

- Species in a niche → taxonomic assignation of the sequences
- Capabilities → in genes directly encoded
- Etc.

# SHOTGUN & AMPLICON

There are two ways to obtain the metagenomics from a complex sample:

- Shotgun metagenomics
- Metabarcoding

### Shotgun metagenomics

-SPECIFIC SPECIES AND GENES

-total number of tRNA genes.

We **sequence random parts** (ideally all of them) of the genomes present in the sample

We can search the **origin of the pieces** (taxonomy, classification) and what **part of genome** they correspong

Given enough piece → complete individual genomes → **MAGs**

**MAGs** assembly requieres a lot of genomic sequences from one organism

Since the sequencing is *random* we need enough **depth** in community sequencing to ensure trustability

It could be really *challenging* when some species aren't that abundant

Requeries *ENOUGH DNA*

↑ High cost

### Metabarcoding

-Just general GENES, only one region of the genome is amplified

↓ Cheaper → we can easily have duplicates or even triplicates

- It is the collection of **small genomic fragments** in the community **amplified by PCR**

Ideally  we just want or need a region to be present only once in every genome, since we are creating amplicons, that "amplify signals, so even small or poor sequences are reported.

if a genome in the community **lacks the region targeted by the PCR primers**, then no amount of sequencing can give us information about that genome

Most popular amplicon used for this methodology are 16S amplicons for Bacteria since every known bacterium has this particular region

### MAIN METHODOLOGY

<img width="499" height="692" alt="image" src="https://github.com/user-attachments/assets/69659899-b2c4-4bd2-b9dc-432e78e05b4e" />

### METADATA

The data about our data: notes on the origin of our samples and how we treated them

# 4 CIENEGAS

Cuatro Ciénegas is an oasis in the Mexican desert whose environmental conditions are often linked to the ones present in ancient seas, due to a higher-than-average content of sulfur and magnesium but a lower concentrations of phosphorus and other nutrients

Compared the differences between the microbial community in its natural, oligotrophic, phosphorus-deficient environment, a pond from the Cuatro Ciénegas Basin (CCB), and the same microbial community under a fertilization treatmen

!! Mean bacterial genome size, GC content, total number of tRNA genes, total number of rRNA genes, and codon usage bias were significantly changed when the bacterial community underwent the treatment.

### METAGENOMICS DATABASES

MG-RAST, MGnify, Marine Metagenomics Portal, Terrestrial Metagenome DB and the GM Repo

### 4 cienegas data

https://www.ncbi.nlm.nih.gov/sra/?term=PRJEB22811

<img width="723" height="228" alt="image" src="https://github.com/user-attachments/assets/bab10994-d22a-4a4d-8e50-62798e32e685" />


# BIO-INFORMATIC WORKFLOWS

The raw reads obtained from the high-throughput sequencing data must pass throfuh several tools to generate the final disired output

Example: 

<img width="765" height="926" alt="image" src="https://github.com/user-attachments/assets/fbf8ea91-2941-40f2-aac1-66475bda280b" />

### QUALITY CONTROL

lets put us on the directory, then unzip the file, and see the first read

    cd ~/dc_workshop/data/untrimmed_fastq/
    gunzip JP4D_R1.fastq.gz
    head -n 4 JP4D_R1.fastq

<img width="1782" height="304" alt="image" src="https://github.com/user-attachments/assets/9ba94697-f7c9-45f2-bcb8-e063fa1bbc9f" />

The numerical value assigned to each character depends on the sequencing platform that generated the reads

 The sequencing machine used to generate our data uses the standard Sanger quality PHRED score encoding, using Illumina version 1.8 onwards

 <img width="764" height="103" alt="image" src="https://github.com/user-attachments/assets/13ef36ad-f950-4583-a04a-16654960264d" />

### Activating an environment

Environments are part of a bioinformatic tendency to do reproducible research

A way to share and maintain our programs in their needed versions used for a pipeline with our colleagues and our future self

CONDA → open-source package and environment management system that runs on Windows, macOS and Linux

    conda activate metagenomics → activates the environment to use FastQC

<img width="846" height="46" alt="image" src="https://github.com/user-attachments/assets/ce4edc40-4bee-4f8b-8e0b-d9d5ba0f0287" />

    fastqc -h → helper menu

<img width="920" height="251" alt="image" src="https://github.com/user-attachments/assets/6f057e56-25df-480c-b73e-11635b70072a" />

### Assessing quality with FastQC

Looks at quality collectively across all reads within a sample

Good quality:

<img width="650" height="487" alt="image" src="https://github.com/user-attachments/assets/b6d14635-844d-4f70-a12d-ce10be2aa672" />


The x-axis displays the base position in the read, and the y-axis shows quality scores

How to read:

-  For each position, there is a box-and-whisker plot showing the distribution of quality scores for all reads at that position (bp).
-  The horizontal red line indicates the median quality score, and the yellow box shows the 1st to 3rd quartile range
-   Background is also color-coded to identify good (green), acceptable (yellow) and bad (red) quality scores.

Bad quality:

<img width="665" height="498" alt="image" src="https://github.com/user-attachments/assets/80e54826-3173-4f45-a551-0db3e6ea3175" />

### ls shortcuts

- a) ls -a → all files even hidden content
- b) ls -S → Fils sorted by size like order
- c) ls -l → metadata, permissions, size, modifications
- d) ls -lh → metadata in human readabñe manner ************
- e) ls -ahlS → All contents with metadata, includding hidden files, sorted by size
    
<img width="733" height="148" alt="image" src="https://github.com/user-attachments/assets/2da40d45-1f01-46f9-ada5-f5ca8842fe8a" />

<img width="751" height="184" alt="image" src="https://github.com/user-attachments/assets/c0a718dd-dbf2-46da-9bc3-7901d19c0d82" />

    
### Running FastQC

FASTQC can accept both zipped and unzipped files

    fastqc *.fastq*
<img width="862" height="260" alt="image" src="https://github.com/user-attachments/assets/b237d544-a553-458e-8b64-1291a2c24ae6" />

<img width="756" height="295" alt="image" src="https://github.com/user-attachments/assets/ab1e0e02-acaa-4533-a426-e56c34013ff1" />

<img width="803" height="266" alt="image" src="https://github.com/user-attachments/assets/ee750011-223e-44fd-9b96-cd2303f5c977" />

    ls 
    
<img width="1326" height="84" alt="image" src="https://github.com/user-attachments/assets/2f097ae4-3a1f-42ef-a6ed-857bda09eb2e" />

The FASTQC, for each input FASTQ file, it created a **".zip"** & **".html"**:

- .zip → multiple output files compressed
- .html → stable webpage displaying the summary report for each sample

### Separate DATA from RESULTS

Create the new directory were to locate the RESULTS

    mkdir -p ~/dc_workshop/results/fastqc_untrimmed_reads 
    
Move the specific files

    mv *.zip ~/dc_workshop/results/fastqc_untrimmed_reads/
    mv *.html ~/dc_workshop/results/fastqc_untrimmed_reads/ 

<img width="1172" height="97" alt="image" src="https://github.com/user-attachments/assets/d6768428-71da-4ec5-951e-d8bdee59f8b7" />

<img width="1774" height="67" alt="image" src="https://github.com/user-attachments/assets/6c54dd52-9413-4cb2-8c0d-3b85c9f2791b" />

### Viewing FASTQC results

<img width="1919" height="1013" alt="image" src="https://github.com/user-attachments/assets/16c99e40-d73e-49ff-b5fd-2ca6e6aae9f5" />


<img width="751" height="376" alt="image" src="https://github.com/user-attachments/assets/80538b4f-7529-4e45-9349-8dec4492f6ba" />

### Other FASTQC outputs

- **Per tile sequence quality**: the machines that perform sequencing are divided into tiles. This plot displays patterns in base quality along these tiles. Consistently low scores are often found around the edges, but hot spots could also occur in the middle if an air bubble was introduced during the run.
- **Per sequence quality scores**: a density plot of quality for all reads at all positions. This plot shows what quality scores are most common.
- **Per base sequence content**: plots the proportion of each base position over all of the reads. Typically, we expect to see each base roughly 25% of the time at each position, but this often fails at the beginning or end of the read due to quality or adapter content.
- **Per sequence GC content**: a density plot of average GC content in each of the reads.
- **Per base N content**: the percent of times that ‘N’ occurs at a position in all reads. If there is an increase at a particular position, this might indicate that something went wrong during sequencing.
- **Sequence Length Distribution**: the distribution of sequence lengths of all reads in the file. If the data is raw, there is often a sharp peak; however, if the reads have been trimmed, there may be a distribution of shorter lengths.
- **Sequence Duplication Levels**: a distribution of duplicated sequences. In sequencing, we expect most reads to only occur once. If some sequences are occurring more than once, it might indicate enrichment bias (e.g. from PCR). This might not be true if the samples are high coverage (or RNA-seq or amplicon).
- **Overrepresented sequences**: a list of sequences that occur more frequently than would be expected by chance.
- **Adapter Content**: a graph indicating where adapter sequences occur in the reads.
K-mer Content: a graph showing any sequences which may show a positional bias within the reads.

### FASTQC text output

lets unzip files

    unzip *.zip

!!! It FAILED, because some of them aren't files are directories, and unzip expect to have just **files**

<img width="1019" height="155" alt="image" src="https://github.com/user-attachments/assets/0c5aee6d-f37b-41ae-98df-a2e974505f90" />

** THE CORRECT WAY**

    for filename in *.zip
    do
    unzip $filename
    done

<img width="1162" height="355" alt="image" src="https://github.com/user-attachments/assets/d6a635c8-3947-4f7b-802a-2fb659783783" />

Here "ls" will show just the *same zipped* directories, but *added other files*

This new files are directories

    ls 
    ls -F → directories are the ones with "/"
    
<img width="1127" height="147" alt="image" src="https://github.com/user-attachments/assets/3490d6be-3137-408a-b0e0-f452f587cb12" />

To see a directory without oppening it: 

    ls -F [directory name]
    ls -F JC1A_R1_fastqc/

<img width="1180" height="79" alt="image" src="https://github.com/user-attachments/assets/c441f2f0-71c4-4924-a7e2-39ad26e39d5c" />

Also for preview summary.txt:

    less JC1A_R1_fastqc/summary.txt

    q → EXIT

<img width="1131" height="350" alt="image" src="https://github.com/user-attachments/assets/f62c1a4f-7cdf-470a-a1f9-65a1cd12bdd6" />

### Document summaries FASTQC

Here we create a file just for documents

Then we use "CAT" to combine several files, from each summary (*/summary.txt) to the new direction (~/dc_workshop/docs/...) with the new file name (...fastqc_summaries.txt)

    $ mkdir -p ~/dc_workshop/docs
    cat */summary.txt > ~/dc_workshop/docs/fastqc_summaries.txt

<img width="1317" height="77" alt="image" src="https://github.com/user-attachments/assets/4db08002-a170-4f88-879b-ab2e3eea418c" />

### Failed tests

Which samples failed at least one of FastQC’s quality tests

    grep FAIL fastqc_summaries.txt

<img width="1351" height="259" alt="image" src="https://github.com/user-attachments/assets/ba31192c-98b9-4a6e-a0f5-de52f5216c1b" />


### MultiQC

a tool that can show the quality of many samples at once.

https://seqera.io/multiqc/

### Automating a quality control workflow

Nano script 

    nano quality_control.sh

Inside the commands

    set -e # This will ensure that our script will exit if an error occurs
    cd ~/dc_workshop/data/untrimmed_fastq/
    
    echo "Running FastQC ..."
    fastqc *.fastq*
    
    mkdir -p ~/dc_workshop/results/fastqc_untrimmed_reads
    
    echo "Saving FastQC results..."
    mv *.zip ~/dc_workshop/results/fastqc_untrimmed_reads/
    mv *.html ~/dc_workshop/results/fastqc_untrimmed_reads/
    
    cd ~/dc_workshop/results/fastqc_untrimmed_reads/
    
    echo "Unzipping..."
    for filename in *.zip
        do
        unzip $filename
        done
    
    echo "Saving summary..."
    mkdir -p ~/dc_workshop/docs
    cat */summary.txt > ~/dc_workshop/docs/fastqc_summaries.txt

# Trimming and filtering

Get rid of sequence data that does not meet our quality standard

Determine the quality threshold we will accept

    trimmomatic → will show you the different versions

► We must specify wheter we have paired-end (PE) or single-end (SE)

► The order in wich we specify the arguments is essential

<img width="1421" height="180" alt="image" src="https://github.com/user-attachments/assets/03e6c34b-4ad7-4ee3-ae78-49c0f368007f" />

### Trimming input-output setting

Trimmomatic will expect **one file as input**, after which you can enter the **optional settings** and, lastly, the **name of the output file**.

<img width="769" height="332" alt="image" src="https://github.com/user-attachments/assets/8323f51f-b83e-4a83-8dec-ab7f2555774b" />

### Trimming parameters

<img width="744" height="422" alt="image" src="https://github.com/user-attachments/assets/b9672b8f-fa3c-4363-92e8-9a9dc8c58a9e" /> <img width="720" height="794" alt="image" src="https://github.com/user-attachments/assets/1046a552-1012-4e91-b623-df98830173ad" />

### EXAMPLE of trimming code

<img width="750" height="146" alt="image" src="https://github.com/user-attachments/assets/61414f60-4920-4ec5-ba14-93b6f354822b" />

<img width="736" height="510" alt="image" src="https://github.com/user-attachments/assets/966b8543-329b-468e-a145-b48b7fa3fb08" />


### Using \ to separate code chunks

    echo he\
    llo\
     worl\
    d

<img width="1057" height="134" alt="image" src="https://github.com/user-attachments/assets/830676b1-e558-46da-9e9c-7fe1d3ab47dc" />

### Running trimmomatic

Check if Universal adapters are present in our sample

In *next-generation sequencing* (NGS), **adapters** are short, synthetic DNA sequences that are ligated to the ends of DNA fragments before sequencing.





























































# ENTER OTHER DIRECTIONS

<img width="1728" height="227" alt="image" src="https://github.com/user-attachments/assets/6397143b-176e-432b-b49f-b5f01dfc4c87" />




    
Alt 126 ~
Alt 92 \
