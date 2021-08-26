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

