# Structural Bioinformatics Workshop resources

This repo contains the resources required for my structural bioinformatics workshop.

There are two versions of the workshop - one version uses Pymol, the other uses the web based protein visualising app NGL.

If you are able to install software on the computer you are using, then I'd recommend using the [Pymol version](./workshop_pymol.md) as Pymol is significantly more powerful and better practice for software you would be using in a proper research role.

Otherwise, use the [NGL version](./workshop_ngl.md) - the instructions are basically the same, but there are a few extra steps in the NGL version (e.g. using an extra webserver to perform the structural alignments.

Also provided are PDF versions of the practical protocols in an easy to print format if you wanted to take notes that way. You can also download the lecture handout as a PDF [here](./Structural_Bioinformatics_Cranfield_2021.pdf) as well.

### If you get stuck...

If things don't work (always a possibility with academic software), the [data](./data) folder contains various files (including the homology model PDB file, called `model.pdb`) so you can use them in a pinch. 

Please - **only use if stuff doesn't work**. Best to try things first.

## Other resources you may find interesting

The big news in structural bioinformatics recently has been Deepmind and their work on Alphafold and Alphafold2. If you are interested in this exciting new approach to modelling, I'd recommend reading the articles/papers on the [Deepmind alphafold page](https://deepmind.com/research/case-studies/alphafold), and perhaps take a look at some of the talks members of the team have done. If you want to really get in the weeds with the details, read the supplementary material to the papers - that is where all the information actually is.

I would be wary, however, of people claiming to have "solved the protein folding problem"... this is a rather grand claim and is not strictly true. They have really come up with a very good solution to the *protein structure prediction problem*. Protein **folding** is a different process that they do not predict IMO. Nonetheless, the software is super impressive and they keep improving it with the release of Alphafold-multimer which can predict complexes.

A really good video explaining the paper in more depth can be found [here](https://www.youtube.com/watch?v=nGVFbPKrRWQ&t=892s). Nice and nerdy, but still understandable. Includes some interesting info on how it was trained as well.

If you want to run Alphafold yourself, there are a number of Google Colab notebooks which allow you to have a go. 

https://colab.research.google.com/github/deepmind/alphafold/blob/main/notebooks/AlphaFold.ipynb

https://github.com/sokrypton/ColabFold

Lots of options. Read the instructions carefully so you understand what is being run.

Typically Colab gives you a GPU with ~12GB of memory - this generally allows the prediction of a protein with 1000 residues. Longer proteins run the risk of running out of memory. So keep that in mind.

The Alphafold team have also set up a [database](https://alphafold.ebi.ac.uk/) in partnership with the EBI. It currently has models "for the human proteome and 20 other key organisms" - this is a really cool resource. They are planning to add ALL Uniref90 proteins in the future, which is a hugely ambitious aim. This database is also cross referenced with the structure section of Uniprot, and Uniprot accession numbers are used to identify alphafold models.

Otherwise, feel free to get in contact with me by raising an issue if you have any questions.

## Using/Adapting this workshop

I have absolutely no issue with people using or adapting content from this workshop for their own students/work. I just ask you give me, Elliot Drew, credit as the original author of the work - a link to this repo would be sufficient.
