# Important 
Here we find the manuscript template: https://docs.google.com/document/d/1l3K5P8ZHNclcVAZ2XyxXIcjhIFgwbyvzgm125V0ioa4/edit?usp=sharing
Whatever we will do, whatever will will write, whatever figures we have all should be placed here and in a central team's drive.
Always use https://citation.crosscite.org/ to reference in APA.

# Workflow
1. Discovering some bioactive products against human pathogenic virus-like Lujo virus and lassa fever etc which all are also emerging viruses and can cause a pandemic situation in the future, and scientists didn't discover any In silico drug till now.

3. We should find out the viral part of that disease protein, then it will be helped to find specific ligands from PubChem, ChemSpider etc. 
We can add some extra flavour to this project, maybe we can take up mutated sequences of a viral protein, model them using AlphaFold (using ColabFold) and check how already existing drugs act against them..?

3. Lujo hemorrhagic fever (LUHF) is caused by Lujo virus, a single-stranded virus of the Arenaviridae family. The limited clinical information about LUHF comes from a small, nosocomial cluster of hemorrhagic disease in September-October 2008 involving 5 patients in South Africa. The case fatality rate was 80% (4/5 cases). We can use the new machine learned methods for drug repurposing studies.

4. **Potential Targets: Lujo virus:** (PDB ID: 6GH8)                                                                                                                             https://www.rcsb.org/structure/6GH8    <br>
                                                                                                                         https://www.nature.com/articles/s41564-018-0224-5 (a very nice paper) 

5. RCSB's Recommended Small Molecules as Ligands
(1)  NAG (2-acetamido-2-deoxy-beta-D-glucopyranose)

6. Literature studies outcomes:
(Ribavirin, HMG-CoA reductase inhibitors (statins), N-acetylcysteine, recombinant factor VIIa)
https://journals.plos.org/plosntds/article?id=10.1371/journal.pntd.0003233 <br> 
https://www.dovepress.com/lujo-virus-current-concepts-peer-reviewed-fulltext-article-VAAT <br>
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4230886/ <br>

7.  **Lassa virus:**
https://www.cell.com/cell/fulltext/S0092-8674(19)30785-8?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS0092867419307858%3Fshowall%3Dtrue <br>
-(PDB ID: 6P91 -viral protein/immune system) https://www.rcsb.org/structure/6P91 <br>
RCSB's Recommended Small Molecules as Ligands (1 Unique) <br>
1. NAG (2-acetamido-2-deoxy-beta-D-glucopyranose)
 
8. -(PDB ID: 6P95 -viral protein/immune system) https://www.rcsb.org/structure/6P95 <br>
RCSB's Recommended Small Molecules as Ligands (1 Unique)
1. NAG (2-acetamido-2-deoxy-beta-D-glucopyranose)
Literature studies outcomes for 6P91 and 6P95: <br>
(Ribavirin+Favipiravir )
https://www.nature.com/articles/s41598-017-10198-0  <br>
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC286250/ <br>
 
# Aim
**6GH8, 6P91 and 6P95 viral protein structures of Lujo and LASSA with ligand Ribavirin. Literature Backed Ligands**
A complete and accurate in-silico drug design approach we will identify potential natural compounds like ribavirin, N-acetylcysteine, etc. against the targeted protein like 6GH8, 6P91, and 6P95, etc, including ADMET, molecular docking, and molecular dynamics (MD) simulation approaches. A total of (100/120/...) natural compounds we will retrieve and analyzing for our studies, with the ADMET properties revealing the efficacy and safety of these compounds, with a total of (finding compounds) violation-free compounds chosen for further evaluation. (Lipinsky rule apply) and the top compounds based on were selected based on their binding affinities. To assess the protein-ligand complex structure's stability, the protein-ligand complex structure we will subject to MD simulations; among these compounds, main ligand compounds exposed the high stability to the protein's binding site.            

Check from literature if there are experimentally verified active residues; don't bother if there is non. 2) Is the target co-crystallized with a native ligand. If so, then you can use DS or Pymol to know the amino acids that have interacted with this ligand but before then make sure that literature says that the ligand has been found to inhibit the target. If non of these work, then we can go on with CASTp or prankweb only for predictions.

# Methods 
(1) Target Protein Identification, Retrieving, and Preparation:
RCSB (https://www.rcsb.org/)

(2) Compound Retrieval and preparation:
PubChem database (https://pubchem.ncbi.nlm.nih.gov/)

(3) Similarity search of ligands:
Ambinter (http://www.ambinter.com/)
 
(4) Active Site Identification:
CASTp (http://sts.bioe.uic.edu/castp/index.html?4jii )

(5) Pharmacokinetics and toxicity (ADMET) properties prediction:
a. Analysis of absorption, distribution, metabolism, and excretion (ADME):
SwissADME (www.swissadme.ch) <br>
b. Analysis of Toxicity:
pkCSM (http://biosig.unimelb.edu.au/pkcsm/) <br>
http://www.way2drug.com/Cell-line/ <br>

(6) Molecular dynamics Simulation:
Desmond (Schrodinger) / GROMACS/ VMD

1 Generation of small molecule derivatives of the best docked phytocompounds
The 3 best docked phytocompounds in the sdf format were uploaded individually to the deep neural networking–based LigDream tool (https://www.playmolecule.org/LigDream/) to generate derivative molecules along with their canonical smiles from each phytocompound.

2. Addition: We can get do the Pharmacophore modeling from (http://zincpharmer.csb.pitt.edu/) and visualize them using http://bioinfo3d.cs.tau.ac.il/PharmaGist/

3. This method is really cool for small molecule screening: https://chemoinfo.ipmc.cnrs.fr/LEA3D/index.html

4. We will then be building QSAR: https://buildqsar.software.informer.com/2.0/  or http://www.way2drug.com/gusar/ and https://mcule.com/

We can also look at: first 1000 molecules in phytolibraries of Indian Medicinal Plants (https://cb.imsc.res.in/imppat/home)  and Traditional Chinese (https://tcmsp-e.com/)

The main methods of viral evolution include point mutations, gene duplication, and viral recombination (Nasir et. al 2012).
1. I can do computational saturation mutagenesis of the viral protein using MutateX (https://github.com/ELELAB/mutatex /https://www.biorxiv.org/content/10.1101/824938v1). MutateX will tell me which point mutation will destabilize the protein structure the most. It will also give me many ways to visualise the data: heatmaps, histograms and a lot of fancy stuff.
However, MutateX will not tell me how protein-ligand interaction will be affected by the mutation. For that I can use mCSM-lig (http://biosig.unimelb.edu.au/mcsm_lig/prediction).
This entire process will be very computationally costly (running MutateX itself might take >24 hours)
and I'm still unclear about many steps in the process.
2.  There is significant reason to suspect that recombination could have given rise to the current Covid-19 pandemic (Patino-Galino et. al 2019). Since we're working on a relatively new virus, it'll be insightful to check the pandemic causing potential of Lujo & Lassa virus using Recombination Detection Program (http://web.cbio.uct.ac.za/~darren/rdp.html)


## Gene-Level analysis - Summary

1.Acquisition of disease-associated targets and candidate genes

Keywords related to viruses were used to search the known target/genes related to the pathogenesis from three major databases, GeneCards (https://www.genecards.org) [15], OMIM (https://omim.org/) [16], and Drugbank database (https://www.drugbank.ca/). To reduce the false positives, only the curated targets that directly associated with the disease were included, and the repetitive targets were removed. The obtained genes were both inputted to draw Venn diagram.(http://bioinformatics.psb.ugent.be/webtools/Venn/), and the intersection genes were collected as candidate genes.

2.Protein-protein interaction (PPI) network

Based on the candidate genes, a PPI network was constructed by importing the candidate genes to the Search Tool for the Retrieval of Interacting Genes (STRING, https://string-db.org/) database, with a highest confidence of 0.9 [17]. Cytoscape software, version 3.8.1 [18] was used to visualize the PPI network. Then, three topological features, “degree”, “betweenness”, and “closeness” were calculated to identify the key genes. 
“Degree” parameter represents the number of edges associated with a node. 
“Betweenness” indicates the number of shortest paths between pairs of nodes, and 
“Closeness” describes the inverse of the number of distances.

3.GO and KEGG pathway enrichment analysis

These data is suppossed to be studied in deep, but for now some important data like Biological Process, Molecular Function, & few Pfam domain is collected and studied from the gene-networks obtained/attached.  
The Gene Ontology (GO) and Kyoto Encyclopedia of Genes and Genomes (KEGG) enrichment were performed by the Database for Metascape (https://metascape.org). GO functionally annotates key genes into three main terms, including cellular components (CCs), molecular functions (MFs), and biological processes (BPs). Besides, Cytoscape ClueGO plugin was employed to further analyze BPs enrichment. KEGG enrichment analysis unveils the possible biological process with key genes. In addition, the bubble chart of GO and KEGG enrichment analysis were performed on the bioinformatics platform (http://www.bioinformatics.com.cn/).

4.Construction of drug-components-disease-targets-pathways network

To characterize the therapeutic mechanisms of ginger for colon cancer, a network of drug-components-disease-targets-pathways was constructed using Cytoscape software, version 3.8.1 [18]. In the network, the nodes with different colors and shapes represent the drug, components, disease, target genes, or disease related pathways, respectively, and an “edge” is an association between the nodes.

A Schematic alternative for finding Drug Compounds :
The key genes identified from the above stage which have good correlation with other genes, active components, and pathways could thus be included in the molecular docking simulation. The PDB-ID of these target genes can be accessed from Protein Data Bank (PDB) database.
 


# EMON
please have a look... :eyes: https://github.com/aakilkhanemon/drug-discovery-project/tree/main/data
 I have attached there target viral protein 3D structure of Lujo and Lassa as PDB format,  control ligand or drugs such as Ribavirin, Favipiravir, Acetylcysteine, Atorvastatin as SDF format (2D & 3D structure),  similar compounds multiple export file as SDF and CSV format of that 4 main ligands or drug using ambinter server (used default of 80% similarity search)                                                                                                                                                                                                                                                                                                                                          6gh8_Lujo_viral_receptor.pdb
6p91_Lassa_viral_receptor.pdb
6p95_Lassa_viral_receptor.pdb
(RSCB: https://www.rcsb.org/)

2D & 3D Conformer_CID_37542_(Ribavirin).sdf
2D & 3D Conformer_CID_492405_(Favipiravir).sdf
2D & 3D Conformer_CID_12035_(Acetylcysteine).sdf
2D & 3D Conformer_CID_60823_(Atorvastatin).sdf
(Pubchem: https://pubchem.ncbi.nlm.nih.gov/ )

multiple_export_(Ribavirin)_similar_ambinter.sdf
multiple_export_(Favipiravir)_similar_ambinter.sdf
multiple_export_(Acetylcysteine)_similar_arbinter.sdf
multiple_export_(Atorvastatin)_similar_ambinter.sdf
(Ambinter: http://www.ambinter.com/)

export_(Acetylcysteine)_similar_arbinter.csv
export_(Atorvastatin)_similar_ambinter.csv
export_(Ribavirin)_similar_ambinter.csv
export_(Favipiravir)_similar_ambinter.csv
(Ambinter: http://www.ambinter.com/) 

Active site determination result for refined Lujo viral protein 6GH8_chain_b using CASTp: http://sts.bioe.uic.edu/castp/index.html?j_612794adc675a  (we will determine active site of our others protein's specific chain receptor using CASTp, because it's so easy) @channel please see the video for understanding of ASD using CASTp

(1) lujo virus main viral protein 6GH8 (carry all chains like a,b,c,d.., ligands, hetatm, water)  (2) refined protein 6GH8 as 6GH8(chain_b)pdf (carry only chain b which is specific and identify for homo sapiens host with carry specific genes[literature study outcome]                                      (3) Pyrx accept that refined protein as macromolecule for protein-ligand docking [no need of energy minimization at all]

we need to store our active site determination results analysis for further studies in the following ms docs. Here I have attached ms template file, please edit the file to fulfill all information as like as screenshot. And go to the link http://sts.bioe.uic.edu/castp/index.html?j_612794adc675a to collect analysis all data such as PocID, Area (SA), Volume (SA), Chain
SeqID, AA, Atom for ms docs.

[Lujo hemorrhagic fever (LUHF) virus] 
Target protein identification, refinement and validation
Target protein identification:
(1) Lujo virus main viral protein 6GH8 downloaded from RCSB (carry all chains like a,b,c,d.., ligands, hetatm, water, etc.)  and save as pdf format rename 6GH8_lujo_viral_protein.
[Uploaded file in Github.(see data section)]
[Tool used: RCSB]
Protein refinement:
(2) Refined protein 6GH8 as 6GH8(chain_b) pdb (carry only chain b which is specific and identify for homo sapiens host with carrying specific genes[literature study outcome]
[Uploaded file in Github.(see data section)]
[Tool used: Biovia Discovery studio]
Protein validation/ energy minimized:
(3) Pyrx accept 6GHB refined protein as macromolecule for protein-ligand docking [no need for energy minimization at all]
[Uploaded pyrx visualized macro molecule image in git hub(see data section)]
[Tool used: Pyrx]
Ligand Identification, Retrieving, and Preparation:
we identify the three best main ligands such as Ribavirin, N-acetylcysteine, Atorvastatin from PubChem databases(downloaded all three's 2D and 3D structure as SDF format) against lujo viral protein according to literature studies outcomes.
To dock Lujo virus viral refined protein 6GH8 (carry only chain b) and specific literature studies outcome of ligands compound such as Ribavirin, N-acetylcysteine, Atorvastatin and it's all similarity compounds collected by ambinter with default as 80% similarity search about 79 (Ribavirin) 96 (N-acetylcysteine) 98 (Atorvastatin) = 273 of total compounds for 6GH8(chain_b) protein docking. From ambinter downloaded multiple export sdf and multiple export csv files of three main ligands Ribavirin, N-acetylcysteine, Atorvastatin.
[uploaded all three multiple export sdf and csv format files in GitHub(see data section)]
[Tool used: Pubchem, Ambinter]
Active site identification and grid box analysis:
Lujo virus viral structure refined protein 6GH8 (chain b) Active site determination result we found most area coverage in pocket ID 1:   5869.075  most volume 3769.615.  The active site started SeqID 87 (GLN-N) to SeqID 196 (THR-CG2) and we set grid box between 87 to 196 amino acid residue. The result is available: http://sts.bioe.uic.edu/castp/index.html?j_612794adc675a
[Uploaded active site determined image from CASTp in GitHub (see data section)]
[Tool used: CASTp]                                   

When we will be eligible to generate docking results through Schrodinger suite and Pyrx, it means we did it almost. To screening 3 main ligands docking scores we will attach 3*4=12 or 3*5= 15 of the compounds (or our mentors suggest) basis on the top docking score in the excel sheet.  Then it's going really easy to get protein-ligand interaction information ( I can manage it to generate 2D/3D/ excel inf. via discovery studio example is there in the figure), ADMET analysis (every member need to collaborate to generate ADMET output, no worry about strategy! step by step procedure share with you all as pdf) of that all top compounds, and finally, need to generate MD simulation studies of that all top compounds via Schrodinger suite or GROMACS.  (@channel please rises your hand if you are familiar with any of MD simulation studies of your interest tool)  At the end of the above all strategy then we can say channel, ''see we've done our job successfully!''  And final to finally the end, we will do together Lujo virus viral protein 6gh8's CADD studies with a beautiful manuscript with the team's fast manuscript writing effort!:heart::100:

Their are two .CSV file one named all details and one inside the dock xp folder. In that all the scores are visible. Also the complete results are in .pjr format when you add that in schrodinger you can see the workspace what I did. Then their is a ligprep file which is the ligand preperation file and prepwizard file which is the protein preperation file. Site map file in that, the sites details with the coordinates and energy present.
I have given 2d image and 3d image of the interaction. If their are two confirmation of ligand   meaning two same ligands having different confirmation binding to the receptor you can see 1 and 2 named at last. I only added readme file for 6gh8 with Ribavirin. Rest which include the favipiravir, acetylcysteine etc follow the same.

