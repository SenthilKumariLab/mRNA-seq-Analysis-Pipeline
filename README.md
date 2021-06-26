# Installation commands for Tool and dependancies used in mRNA-seq-Analysis-Pipeline 
#Intallation of Tolls
#Installation of Cutadapt
sudo apt install python3-cutadapt
#Installation of STAR Aligner
# Get latest STAR source from releases
wget https://github.com/alexdobin/STAR/archive/2.7.9a.tar.gz
tar -xzf 2.7.9a.tar.gz
cd STAR-2.7.9a
## Compile STAR
cd STAR/source
make STAR
#Installation of FeatureCounts
sudo apt-get update
sudo apt-get install subread
#Installation of R-base
sudo apt-get install r-base
#Installation of EdgeR
R
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("edgeR")
#Installation of Dependancies
install.packages("readr")
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("HTSFilter")
install.packages("calibrate")
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("EnhancedVolcano")
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("fgsea")
install.packages("tibble")
install.packages("ggplot2")

