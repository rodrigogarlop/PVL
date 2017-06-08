Appendix Tables and Accesory Figures
First version: May 30th, 2017
Update last version: Jun 8th, 2017
	-All Figures are now in .pdf format for better compatibility
	-Files have been renamed to be self explanatory

THE APPENDIX:
This GitHub project, "PVL", contains the Appendix/accessory-files for the bioinformatic analyses of the PhD thesis "Study of the oral virome and microbiome associated to the proliferative verrucous leukoplakia" by Rodrigo Garcia Lopez, directed by Prof. Andres Moya and Dr. Vicente Perez Brocal.

The manuscript contains no traditional appendix as several tables and figures were too large for printing. Thus, as an alternative, an online repository was created at the address: https://github.com/rodrigogarlop/PVL

Although files can be previewed online, it is advisable to download them for zooming-in. All contingency tables (.txt files) can be opened in Excel/Calc spreadsheets or similar software for better viewing. In Windows, files in .txt format do not open correctly in Notepad. These are best displayed on Notepad++ (which can be downloaded from https://notepad-plus-plus.org/download/v7.3.3.html).

A directory index can be found in Appendix_directories.pdf
A file index can be found in Appendix_contents.pdf

The directory structure follow the manuscript order:
01 - Composition
These folders contain the complete collection of composition stacked bar plots at every taxonomic level available (domain, phylum, class, order, family, genus, and species for non-viral sets and type, Baltimore, order, class, family, subfamily, genus, and species in viral sets).
Separate sets were used for different subsets in the WGS sets:
all - It contains all items in a WGS sets
bact - It contains only bacteria and archaea records from the WGS sets
fungi - It contains only fungi records from the WGS sets
non_vir - It contains all records other than viral ones from the WGS sets
other - It contains all records other than viral and bacterial hits from the WGS sets
proph - It contains only prophage records from the WGS sets
vir - It contains only viral records form the WGS sets. In the DNA set, this one also includes bacteriophages

02 - Rarefaction Curves
This folder contains the rarefaction curves (cummulative abundance) from the three main datasets> the 16S profiles, and the two WGS, cDNA and DNA. Each has a figure and a legend

03 - Alpha Diversity
This folder contains the alpha diversity comparison for each of the three main sets (16S, cDNA and DNA). They were rarefied at 3000 observations to a total of 1000 iterations. Raw results by sample in both the chao1 and the shannon index are summarized in boxplot graphs chao1_3000_all_samples.pdf and shannon_3000_all_samples.
The comparisons by each of the indexes and the total observed items are included in separate folders, each grouping the samples by age group, by pathologic group ("group") and by sample location. Boxplots of the comparisons are included as well as their statistic comparison (e.g. Group_boxplots.pdf and Group_stats.txt, respectively).

04 - Beta Diversity
This folder contains the Principal Coordinate Analysis (PCoA) plots and statistical comparisons for each of the five subsets in the beta diversity analyses: 16S, cDNA_nonvir, cDNA_vir, DNA_nonvir, and DNA_vir. Each set contains both a Bray_Curtis and a Jaccard folder, containing the results of the analyzis built with the corresponding matrix. 
In each separate type-of-distance folder there is:
PCoA_plot folder - This contains an index.html file and a folder called "emperor_required_resources". Both of them are required to open the 3d PCoA plots using the .html file (firefox or chrome).
Comparison_between_groups - This contains boxplot graphs and statistics from grouped distances within each group depending on sample grouping (group, gender, by pathologic group ["group"] and by sample location). Two-sided Student's two-sample t-tests are between al permutations are reported in the tables (_Stats.txt files).
Support-by-group (Only in Bray_Curtis folders) - It contains the adonis test results for the age group, the pathologic group and the sample location independently.

05 - Heatmaps
This folder contains the heatmaps for each of the five main datasets (16S, cDNA_nonvir, cDNA_vir, DNA_nonvir, and DNA_vir) at each taxonomic/classification level (different for viruses as stated before). Graphics were only created if there was more than one category (e.g. no Domain level heatmap exists for the 16S set). Only the last category appears in each row. They were ordered by groups (PVL, OL, OSCC, CTRL).

06 - Differential Abundance
This folder contains the results of the three methods used to compare the different groups to find differential abundance of any recods.
LEfSe results were only obtained for nonviral records (no relevant biomarkers were found in the viral sets). For each set, the results include:
LEfSe.pdf - This file has the differentially abundant markers at any taxonomic level that have a high LDA score (>2 log scale). These were compared by pathologic group (PVL, OL, OSCC, CTRL).
Cladogram.pdf - This contains a cladogram displaying overrepresented markers in each group at different taxonomic levels. This could not be created for the cDNA_nonvir set.
The Kruskall-Wallis-Group_significance folder contains the tabular results of such test as carried out for each group (group, gender, by pathologic group ["group"] and by sample location) as well as sample-corrected p-values. A set of each group is included for each of the five datasets.
The DESeq2 negative binomial tabular results contains the results of the paired comparisons between the pathologic groups in each of the datasets considering the permutations: OL versus CTRL, OSCC versus CTRL, OSCC versus OL, PVL versus CTRL, PVL versus OL, and PVL versus OSCC. Adjusted p-values are included.

07 - Tables
This folder contains the contingency tables at different stages of the process.
The Raw folder contains collated 16S records (at the OTU/species level), the cDNA and DNA with no human included and only record with more than 10 apperances and at least found in 2 samples.
The Split domain folder contains the collection of tables from the split cDNA and DNA datasets. These include the all, bact, fungi, non_vir, other, proph, and vir tables subsets that are described in folder 01 of this document.
The Strict folder contains tables that were filtered further to remove those records that did not appear in at least 10 samples or were in low abundance.

