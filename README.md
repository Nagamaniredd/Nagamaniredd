- 👋 Hi, RAHUL
Yersinia Protein Analysis Project
Overview
This research project aims to investigate the presence, conservation, and functional aspects of key proteins (Endolysin and Holin) in Yersinia strains, specifically focusing on NewYersinia1 and NewYersinia2. The study explores their potential role in Yersiniosis, an acute enteric disease caused primarily by Yersinia enterocolitica.
Methods
1. Sequence Retrieval
•	Nucleotide database search on NCBI using the term "Tc-PAIye" to identify relevant sequences.
•	Downloading and storing sequences for further analysis.
2. BLAST Analysis
•	Utilizing BLAST software to identify homologous genes in the NewYersinia genomes.
•	Commands for database conversion and sequence searching.
3. Python Scripting
•	Writing a Python script using Biopython for efficient sequence searching.
•	Installation and usage instructions for Anaconda and JupyterLab.
4. Physio-Chemical Analysis
•	Utilizing ProtParam tool for approximating physical and chemical properties of proteins.
•	Assessing molecular weight, GRAVY score, aliphatic index, amino acid composition, etc.
5. Protein Structure Modeling
•	Using SwissModel for modeling protein structures.
•	Uploading target sequences and analyzing model quality.
6. MSA and Phylogenetic Tree Construction (To be worked on)
•	Planning to use Mega XI for Multiple Sequence Alignment (MSA) and phylogenetic tree construction.
7. Conserved Domain Database (CDD) Search
•	Running protein sequences in the CDD tool to identify conserved domains.
•	Providing insights into the functional aspects of the proteins.
Results and Analysis

from Bio import SeqIO

sequence_found = Falsewhile not sequence_found:
    # User should have file in the directory that they are running their code from    file_name = input("File name with extension: ")
    file_type = input("File type: ")
    seq_ID_q = input("Give the sequence ID you are looking for: ")

    try:
        for record in SeqIO.parse(file_name, file_type):
            if seq_ID_q in record.id:
                print(record)
                sequence_found = True        if not sequence_found:
            print("This sequence ID does not exist in your file")

    except (FileNotFoundError, ValueError):
        print("This file doesn't exist in this directory")
NewYersinia1
•	Detailed BLAST results for i-spanin, o-spanin, Endolysin, and Holin.
•	Conserved Domain Database (CDD) search results.
•	Protein structure modeling outcomes.
NewYersinia2
•	BLAST and CDD results for i-spanin, Endolysin, and Holin.
•	Protein structure modelling outcomes.
Discussion
•	Unravelling the evolutionary context and functional implications of Yersinia proteins.
•	Clade formation in the phylogenetic tree and potential evolutionary alliances.
•	Significance of conserved domains in understanding protein functions.
Conclusion
•	Summarizing the key findings and their implications for understanding Yersinia pathogenesis.

	



<
