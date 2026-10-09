**Introduction to Bioinformatics: Definition, Branches, Applications, and Outlook**

*Dr.rer.nat. Arli Aditya Parikesit, S.Si., M.Si. | Department of Biotechnology, i3L University, Jakarta*

**1\. Definition of Bioinformatics**

Bioinformatics uses computational methods to store, organise, analyse and interpret biological data. Luscombe, Greenbaum and Gerstein separated it from computational biology. In their view, bioinformatics concerns the handling of biological data and the tools that extract information from it, while computational biology uses models to test biological questions \[1\]. Their working definition frames the field as conceptualising biology in terms of macromolecules and then applying informatics techniques from applied mathematics, computer science and statistics to organise the information associated with those molecules on a large scale \[1\]. The two overlap heavily in practice.

The field draws on biology, computer science and statistics. Pevsner describes it as the step that turns raw sequences and measurements into biological knowledge \[2\]. Lesk traces its growth to the need for managing sequence databases as they expanded \[3\].

The word itself predates the genome era. Hogeweg recalls that she and Ben Hesper began using it in the early 1970s for the study of informatic processes in biotic systems, and she argues that this broader meaning is re-emerging \[4\]. From the late 1980s the term mostly referred to comparative analysis of genome data \[4\]. BLAST, published in 1990, is a typical tool of that period: a fast heuristic for finding local similarity between a query and a sequence database \[5\].

**2\. Branches of Bioinformatics**

Several branches now have enough material to be taught as separate subjects. Sequence bioinformatics covers alignment, gene prediction and phylogenetic reconstruction \[2,3,5\]. Structural bioinformatics works with three-dimensional macromolecules. AlphaFold predicted protein structures with accuracy that, in many cases, approaches experimental methods \[6\]. Transcriptomics analyses gene expression from RNA sequencing, and count-based models such as DESeq2 are a common choice for finding differentially expressed genes \[7\]. DESeq2 fits generalised linear models to count data and moderates fold-change estimates, which helps when replicate numbers are small or counts are low \[7\]. Pathway resources such as KEGG connect these layers to biological function, because the knowledge base links genomic information with higher-order functional information \[8\].

Systems bioinformatics studies how components combine into functioning cells. Kitano described systems biology as the study of the structure and dynamics of cellular and organismal function, and he identified robustness as a property that emerges at the system level \[9\]. Computational work in this branch assembles networks from interaction data and asks how their topology relates to function. Barabási and Oltvai reviewed how metabolic and protein interaction networks share organising features such as highly connected hubs \[10\]. Constraint-based models add a quantitative layer. Flux balance analysis, for example, combines the stoichiometric matrix of a metabolic network with linear programming to calculate metabolite flow, and it needs no kinetic parameters \[11\].

Theoretical biology supplies the mathematical models that the data analysis branches later test. Hogeweg places the origin of bioinformatics in this tradition and points to Kauffman's random Boolean networks, which introduced large-scale transcription regulation networks and treated a cell type as an attractor of a dynamical system \[4\]. In his 1969 analysis, randomly wired genetic nets in which each gene has two or three inputs behaved in an orderly and stable way, and the number of behavioural modes per net roughly predicted the number of cell types in an organism \[12\]. Such models leave out most molecular detail, yet they yield quantitative predictions about stability, cell fate and the effect of noise.

Epigenetics adds a regulatory layer that the DNA sequence does not carry by itself. Allis and Jenuwein describe how two decades of work on chromatin-modifying enzymes turned epigenetics from a set of curious phenomena into a functionally dissected field \[13\]. DNA methylation is the mark most often analysed computationally. Bird reviewed how methylation patterns are established and then maintained through cell division, which gives them a role as a form of cellular memory \[14\]. Analysis tools follow the assay. Bismark maps bisulfite-converted reads and calls cytosine methylation in a single step, and its output separates CpG, CHG and CHH contexts \[15\]. For Infinium arrays, minfi offers preprocessing, quality assessment and detection of differentially methylated regions \[16\]. At the reference level, the Roadmap Epigenomics Consortium analysed 111 human epigenomes profiled for histone modifications, DNA accessibility, DNA methylation and RNA expression \[17\].

Protein domain annotation links sequence analysis to structure and evolution. Dr. Parikesit's doctoral work applied domain annotation across the three domains of life, and his current interests include immunoinformatics, in silico drug design, in silico transcriptomics and artificial intelligence \[18\]. These interests overlap with the branches above, mainly structural bioinformatics and transcriptomics and, through the group's public repositories, epigenetics (Section 3).

**3\. Applications**

Computational screening is most useful when it narrows candidates before expensive laboratory work. One recent study screened 25 compounds from Indonesian ethnopharmacological reports against Plasmodium falciparum CDPK2 \[19\]. No CDPK2 structure was deposited in the PDB at the time, so the authors modelled the protein from its sequence, docked the ligands with the AutoDock Vina method in YASARA, ran density functional theory calculations on the best-scoring ligands in ORCA, and assessed the most promising complex by normal mode analysis \[19\]. A second in silico study examined known RNA polymerase inhibitors against the RdRp of Rift Valley fever virus \[20\]. The four best candidates showed binding affinities equal to or higher than the control, favipiravir, and molecular dynamics fluctuation plots indicated stable protein-ligand interactions \[20\]. Both give computational leads that still need experimental confirmation.

Bioinformatics also supports data pipelines that others can reuse. Public GitHub repositories from this group include pipelines for TCGA epigenetic data, Alzheimer's disease epigenetic mining and Plasmodium protein domain annotation \[21\]. Sequence mining has also been applied to non-model organisms. Wicaksono and colleagues used homology-based in silico methods on published omics data from *Sapria himalayana* and *Rafflesia cantleyi* and found that 7 of 9 highly conserved plant miRNA families are present in Rafflesiaceae, with 22 variants in total \[22\]. These plants are solely parasitic on Tetrastigma vines, and the genetics of their crosstalk with the host remains unexplored, so a catalogue of conserved miRNAs gives a starting point \[22\].

**4\. Outlook**

I see four trends shaping the next decade. This is my own reading and not a settled consensus. First, deep learning is moving from prediction into design. DeepMind's structure system drew wide attention because its results were competitive with experiment \[6,23\], and AlphaFold 3 extends the approach to complexes of proteins, nucleic acids, small molecules and ions \[24\]. Second, data volume keeps growing. Stephens and colleagues compared genomics with astronomy, YouTube and Twitter and judged genomics to be on par with, or more demanding than, the others in acquisition, storage, distribution and analysis \[25\]. Third, the layers described above will be modelled together more often. Network, constraint-based and epigenomic approaches \[10,11,17\] each describe one layer of the same cell, and joint models should make the regulatory and metabolic consequences of a change easier to follow. Fourth, reproducibility is becoming a requirement. The FAIR principles ask that data and other digital research artefacts be findable, accessible, interoperable and reusable, and they guide the evaluation of implementation choices without prescribing a technology \[26\]. The main risk is over-trusting model output. A predicted structure or docking score is a hypothesis that needs experimental testing.

**5\. References**

\[1\] Luscombe, N. M., Greenbaum, D., & Gerstein, M. (2001). What is bioinformatics? A proposed definition and overview of the field. Methods of Information in Medicine, 40(4), 346–358. https\://doi.org/10.1055/s-0038-1634431

\[2\] Pevsner, J. (2015). Bioinformatics and Functional Genomics (3rd ed.). Wiley-Blackwell.

\[3\] Lesk, A. M. (2014). Introduction to Bioinformatics (4th ed.). Oxford University Press.

\[4\] Hogeweg, P. (2011). The roots of bioinformatics in theoretical biology. PLoS Computational Biology, 7(3), e1002021. https\://doi.org/10.1371/journal.pcbi.1002021

\[5\] Altschul, S. F., Gish, W., Miller, W., Myers, E. W., & Lipman, D. J. (1990). Basic local alignment search tool. Journal of Molecular Biology, 215(3), 403–410. https\://doi.org/10.1016/S0022-2836(05)80360-2

\[6\] Jumper, J., Evans, R., Pritzel, A., et al. (2021). Highly accurate protein structure prediction with AlphaFold. Nature, 596(7873), 583–589. https\://doi.org/10.1038/s41586-021-03819-2

\[7\] Love, M. I., Huber, W., & Anders, S. (2014). Moderated estimation of fold change and dispersion for RNA-seq data with DESeq2. Genome Biology, 15(12), 550\. https\://doi.org/10.1186/s13059-014-0550-8

\[8\] Kanehisa, M., & Goto, S. (2000). KEGG: Kyoto Encyclopedia of Genes and Genomes. Nucleic Acids Research, 28(1), 27–30. https\://doi.org/10.1093/nar/28.1.27

\[9\] Kitano, H. (2002). Systems biology: a brief overview. Science, 295(5560), 1662–1664. https\://doi.org/10.1126/science.1069492

\[10\] Barabási, A.-L., & Oltvai, Z. N. (2004). Network biology: understanding the cell's functional organization. Nature Reviews Genetics, 5(2), 101–113. https\://doi.org/10.1038/nrg1272

\[11\] Orth, J. D., Thiele, I., & Palsson, B. Ø. (2010). What is flux balance analysis? Nature Biotechnology, 28(3), 245–248. https\://doi.org/10.1038/nbt.1614

\[12\] Kauffman, S. A. (1969). Metabolic stability and epigenesis in randomly constructed genetic nets. Journal of Theoretical Biology, 22(3), 437–467. https\://doi.org/10.1016/0022-5193(69)90015-0

\[13\] Allis, C. D., & Jenuwein, T. (2016). The molecular hallmarks of epigenetic control. Nature Reviews Genetics, 17(8), 487–500. https\://doi.org/10.1038/nrg.2016.59

\[14\] Bird, A. (2002). DNA methylation patterns and epigenetic memory. Genes & Development, 16(1), 6–21. https\://doi.org/10.1101/gad.947102

\[15\] Krueger, F., & Andrews, S. R. (2011). Bismark: a flexible aligner and methylation caller for Bisulfite-Seq applications. Bioinformatics, 27(11), 1571–1572. https\://doi.org/10.1093/bioinformatics/btr167

\[16\] Aryee, M. J., Jaffe, A. E., Corrada-Bravo, H., Ladd-Acosta, C., Feinberg, A. P., Hansen, K. D., & Irizarry, R. A. (2014). Minfi: a flexible and comprehensive Bioconductor package for the analysis of Infinium DNA methylation microarrays. Bioinformatics, 30(10), 1363–1369. https\://doi.org/10.1093/bioinformatics/btu049

\[17\] Roadmap Epigenomics Consortium, Kundaje, A., Meuleman, W., Ernst, J., et al. (2015). Integrative analysis of 111 reference human epigenomes. Nature, 518(7539), 317–330. https\://doi.org/10.1038/nature14248

\[18\] Parikesit, A. A. Faculty profile: Dr.rer.nat. Arli Aditya Parikesit, S.Si., M.Si. i3L University. https\://i3l.ac.id/indonesia-international-institute-for-life-sciences/about-i3l/faculty-members/dr-rer-nat-arli-aditya-parikesit-s-si-m-si/ (accessed 9 October 2026\)

\[19\] Gholam, G. M., Dwicesaria, M. A., Artika, I. M., et al. (2025). Indonesian herbal compounds as potential inhibitors of Plasmodium falciparum CDPK2: Insights from docking, molecular dynamics, and DFT analysis. Journal of Pharmacy & Pharmacognosy Research, 13(S1), S289–S302. https\://doi.org/10.56499/jppres25.2336\_13.s1.289

\[20\] Lorell, J., Gautama, N. R. P., Tanzil, T. S., Subagja, M., & Parikesit, A. A. (2025). In silico study of RNA polymerase inhibitor drugs for Rift Valley fever virus using RdRp protein as the target. Journal of Pharmacy and Pharmacognosy Research, 13(1), 1–15. https\://doi.org/10.56499/jppres24.1967\_13.1.1

\[21\] Parikesit, A. A. GitHub profile (Johnkecops), repositories Epigenetics, Alzheimer\_Epigenetics and Plasmodium\_Protein\_Domain\_Annotation. https\://github.com/Johnkecops (accessed 9 October 2026\)

\[22\] Wicaksono, A., Meitha, K., Wan, K. L., Mat Isa, M. N., Parikesit, A. A., & Molina, J. (2025). Hairpin in a haystack: In silico identification and characterization of plant-conserved microRNA in Rafflesiaceae. Open Life Sciences, 20(1), 20221033\. https\://doi.org/10.1515/biol-2022-1033

\[23\] Callaway, E. (2020). 'It will change everything': DeepMind's AI makes gigantic leap in solving protein structures. Nature, 588(7837), 203–204. https\://doi.org/10.1038/d41586-020-03348-4

\[24\] Abramson, J., Adler, J., Dunger, J., et al. (2024). Accurate structure prediction of biomolecular interactions with AlphaFold 3\. Nature, 630(8016), 493–500. https\://doi.org/10.1038/s41586-024-07487-w

\[25\] Stephens, Z. D., Lee, S. Y., Faghri, F., et al. (2015). Big data: Astronomical or genomical? PLoS Biology, 13(7), e1002195. https\://doi.org/10.1371/journal.pbio.1002195

\[26\] Wilkinson, M. D., Dumontier, M., Aalbersberg, I. J., et al. (2016). The FAIR Guiding Principles for scientific data management and stewardship. Scientific Data, 3, 160018\. https\://doi.org/10.1038/sdata.2016.18