# Introduction to Bioinformatics: Definition, Branches, Applications, and Outlook

*Dr.rer.nat. Arli Aditya Parikesit, S.Si., M.Si. | Department of Bioinformatics, i3L University, Jakarta*

## 1. Definition of Bioinformatics

Bioinformatics uses computational methods to store, organise, analyse and interpret biological data. Luscombe, Greenbaum and Gerstein separated it from computational biology. In their view, bioinformatics concerns the handling of biological data and the tools that extract information from it, while computational biology uses models to test biological questions [1]. The two overlap heavily in practice.

The field draws on biology, computer science and statistics. Pevsner describes it as the step that turns raw sequences and measurements into biological knowledge [2]. Lesk traces its growth to the need for managing sequence databases as they expanded [3].

## 2. Branches of Bioinformatics

Several branches now have enough material to be taught as separate subjects. Sequence bioinformatics covers alignment, gene prediction and phylogenetic reconstruction [2,3]. Structural bioinformatics works with three-dimensional macromolecules. AlphaFold predicted protein structures with accuracy that, in many cases, approaches experimental methods [4]. Transcriptomics analyses gene expression from RNA sequencing, and count-based models such as DESeq2 are a common choice for finding differentially expressed genes [5]. Pathway resources such as KEGG connect these layers to biological function [6].

Protein domain annotation links sequence analysis to structure and evolution. Dr. Parikesit's doctoral work applied domain annotation across the three domains of life, and his current interests include immunoinformatics, in silico drug design, in silico transcriptomics and artificial intelligence [7]. These are the branches where his group's projects sit.

## 3. Applications

Computational screening is most useful when it narrows candidates before expensive laboratory work. One recent study screened Indonesian herbal compounds against *Plasmodium falciparum* CDPK2 using docking, molecular dynamics and density functional theory [8]. A second in silico study examined RNA polymerase inhibitors against the RdRp of Rift Valley fever virus [9]. Both give computational leads that still need experimental confirmation.

Bioinformatics also supports data pipelines that others can reuse. Public GitHub repositories from this group include pipelines for TCGA epigenetic data, Alzheimer's disease epigenetic mining and *Plasmodium* protein domain annotation [10]. Sequence mining has also been applied to non-model organisms. Wicaksono and colleagues used in silico methods to identify and characterise plant-conserved microRNAs in Rafflesiaceae [11].

## 4. Outlook

I see three trends shaping the next decade, though this is my own reading rather than a settled consensus. First, deep learning is moving from prediction into design. DeepMind's structure system drew wide attention because its results were competitive with experiment [4,12]. Second, data volume keeps growing. Stephens and colleagues estimated that genomic data could reach the exabyte range, putting biology among the largest data producers [13]. Third, reproducibility is becoming a requirement. The FAIR principles ask that data and code be findable, accessible, interoperable and reusable [14]. The main risk is over-trusting model output. A predicted structure or docking score is a hypothesis to test, not a result.

## 5. References

[1] Luscombe, N. M., Greenbaum, D., & Gerstein, M. (2001). What is bioinformatics? A proposed definition and overview of the field. *Methods of Information in Medicine*, 40(4), 346–358.

[2] Pevsner, J. (2015). *Bioinformatics and Functional Genomics* (3rd ed.). Wiley-Blackwell.

[3] Lesk, A. M. (2014). *Introduction to Bioinformatics* (4th ed.). Oxford University Press.

[4] Jumper, J., Evans, R., Pritzel, A., et al. (2021). Highly accurate protein structure prediction with AlphaFold. *Nature*, 596, 583–589. https://doi.org/10.1038/s41586-021-03819-2

[5] Love, M. I., Huber, W., & Anders, S. (2014). Moderated estimation of fold change and dispersion for RNA-seq data with DESeq2. *Genome Biology*, 15, 550. https://doi.org/10.1186/s13059-014-0550-8

[6] Kanehisa, M., & Goto, S. (2000). KEGG: Kyoto Encyclopedia of Genes and Genomes. *Nucleic Acids Research*, 28(1), 27–30. https://doi.org/10.1093/nar/28.1.27

[7] Parikesit, A. A. Faculty profile: Dr.rer.nat. Arli Aditya Parikesit, S.Si., M.Si. i3L University. https://i3l.ac.id/indonesia-international-institute-for-life-sciences/about-i3l/faculty-members/dr-rer-nat-arli-aditya-parikesit-s-si-m-si/ (accessed 9 October 2026)

[8] Gholam, G., Dwicesaria, M., Artika, I., et al. (2025). Indonesian herbal compounds as potential inhibitors of *Plasmodium falciparum* CDPK2: Insights from docking, molecular dynamics, and DFT analysis. *Journal of Pharmacy & Pharmacognosy Research*, 13, S289–S302. https://doi.org/10.56499/jppres25.2336_13.s1.289

[9] Lorell, J., Gautama, N. R. P., Tanzil, T. S., Subagja, M., & Parikesit, A. A. (2025). In silico study of RNA polymerase inhibitor drugs for Rift Valley fever virus using RdRp protein as the target. *Journal of Pharmacy and Pharmacognosy Research*, 13(1), 1–15. https://doi.org/10.56499/jppres24.1967_13.1.1

[10] Parikesit, A. A. GitHub profile (Johnkecops), repositories Epigenetics, Alzheimer_Epigenetics and Plasmodium_Protein_Domain_Annotation. https://github.com/Johnkecops (accessed 9 October 2026)

[11] Wicaksono, A., Meitha, K., Wan, K. L., Mat Isa, M. N., Parikesit, A. A., & Molina, J. (2025). Hairpin in a haystack: In silico identification and characterization of plant-conserved microRNA in Rafflesiaceae. *Open Life Sciences*, 20(1), 20221033. https://doi.org/10.1515/biol-2022-1033

[12] Callaway, E. (2020). 'It will change everything': DeepMind's AI makes gigantic leap in solving protein structures. *Nature*, 588, 203–204. https://doi.org/10.1038/d41586-020-03348-4

[13] Stephens, Z. D., Lee, S. Y., Faghri, F., et al. (2015). Big data: Astronomical or genomical? *PLoS Biology*, 13(7), e1002195. https://doi.org/10.1371/journal.pbio.1002195

[14] Wilkinson, M. D., Dumontier, M., Aalbersberg, I. J., et al. (2016). The FAIR Guiding Principles for scientific data management and stewardship. *Scientific Data*, 3, 160018. https://doi.org/10.1038/sdata.2016.18
