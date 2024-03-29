# DREPAL-IPCINGSTOOLKIT

IPCINGSTOOLKIT is an NGS analysis toolkit.

IPCINGSTOOLKIT was developed to aid in the analysis of next generation sequencing data. Users can do the following with this APP:

* Import sequences  
* Remove adapters, low quality bases/positions, and perform read-level QC 
* Align paired-end sequencing reads to the human reference genome.
* Extract unmapped/unaligned reads.
* Visualize the part of each element in the sequence 
* Split bam files into forward and reverse reads.
* Generate VCF file
* Get SNPs Matrix


Dependencies: 

The IPCINGSTOOLKIT APP contains a pipeline requires the following dependencies:

* Fastp
* sickle
* Fastqc 
* BWA 
* Samtools
* Bcftools
* Picard

IPCINGSTOOLKIT was built with streamlit python librairie  .....

## Installation

### 1.  Root mode

```
sudo -i
```
```
cd /home/xxxxxx/
```
go to **/home/xxxxxxx/** 
- xxxxxx is current user path example : */home/stanlasso/

### 2. IPCINGSTOOLKIT

To complete installation of IPCINGSTOOLKIT  clone the directory and enter it.

```
git clone git@github.com:stanlasso/DREPAL-IPCINGSTOOLKIT.git
```
### 3. Conda

This APP requires conda to be installed and available on the system.

To do this install conda via the miniconda installers found [here](https://docs.conda.io/en/latest/miniconda.html) and instructions [here](https://docs.conda.io/projects/continuumio-conda/en/latest/user-guide/install/index.html).
 

#### Linux

  To obtain the installer for linux use the following:
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

  Then, install miniconda,

```
sh Miniconda3-latest-Linux-x86_64.sh
```

#### MacOS

  To obtain the installer for MacOS, you can [download](https://docs.conda.io/en/latest/miniconda.html) it manually or use wget:
```
wget https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
```

  Then, install miniconda,

```
sh Miniconda3-latest-MacOSX-x86_64.sh
```

### 4. Make Bioinfo ENV and install sickle
```
conda env create -f DEVAPP.yml
```
```
conda activate DEVAPP
```
```
sudo apt-get install -y sickle
```
### 5.Make and activate streamlit ENV

- install virtualenv [Python version >=3.8]
```
sudo apt install python3-virtualenv 
```
- make env
```
virtualenv myenv
```
- activate myenv
```
source myenv/bin/activate
```
- install packages with requirment.txt
```
pip install -r requirment.txt
```
### 6. Run APP
```
streamlit run APP/app.py --server.maxUploadSize=42000

```
### 7. Open Web Browser and Paste addresse
*localhost:xxxx 
- xxxx is a default port 

# Contributions

- Egomli Stanislas ASSOHOUN 
- Aristide Berenger AKO 
- Christian-Renaud SERY
- Kablan Jerôme ADOU
- Catherine DOUGA
- Ronan JAMBOU 
