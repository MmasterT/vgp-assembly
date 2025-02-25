# vgp-assembly
VGP repository for the genome assembly working group

## Contents
* DNAnexus Workflow
* Docker images with WDL Workflow
* Pipeline for local run
* MitoVGP pipeline
* Instructions for AWS s3 genomeark
* Meta data
* Citation
 
 
## DNAnexus Workflow
 
The production of the VGP assemblies is performed on DNAnexus, which is available for anyone that registers.
We welcome new trainees who are interested in leading the assembly of VGP and other genomes. Feel free to contact us.
* [Tutorials](https://github.com/VGP/vgp-assembly/blob/master/tutorials/DNAnexus_workflow_1.7_tutorial.md): starting point for new trainees
* [Workflows](https://github.com/VGP/vgp-assembly/tree/master/dx_workflows): workflow to run each assembly steps
* [Applets](https://github.com/VGP/vgp-assembly/tree/master/dx_applets): individual applets in the workflow
* [Retrieve job info](https://github.com/VGP/vgp-assembly/tree/master/dx_scripts)
 
 
## Docker images with WDL Workflow
 
The scaffolding pipeline to run on generic architecture and Docker containers is available to the public. This includes a WDL implementation of the scaffolding portion of VGP Assembly, as well as some of the QC steps. Note that Falcon assembly and Arrow polishing are not included.
 
* [WDL Pipeline](https://github.com/VGP/vgp-assembly/blob/master/wdl_pipeline/WDL_Manual.md): read the manual first
 
 
## Pipeline for local run
 
The local pipeline is available for each individual step for scaffolding, polishing, and evaluation as bash scripts. These scripts were used to locally assemble the first 17 genomes described in [Rhie et al. 2021](https://doi.org/10.1038/s41586-021-03451-0).
 
Note the scripts are optimized to run on a Slurm schedular and tested on [Biowulf](https://hpc.nih.gov/). All submitter scripts have a prefix of `_submit_`.
 
* [Pipeline](https://github.com/VGP/vgp-assembly/tree/master/pipeline)
 
## MitoVGP pipeline
 
Pipeline for generating mitochondrial sequences is available on a conda release.
* [MitoVGP](https://github.com/VGP/vgp-assembly/tree/master/mitoVGP)
 
 
## Instructions for AWS s3 genomeark
 
This is only relevant for our collaborators and data managers, for sharing sequencing data on genomeark not produced by VGP.
* [Upload to genomeark](https://github.com/VGP/vgp-assembly/tree/master/aws_upload)
* [Symlink s3 objects to DNAnexus](https://github.com/VGP/vgp-assembly/tree/master/AWS_bucket)
* [Data structure on AWS genomeark and DNAnexus](https://github.com/VGP/vgp-assembly/blob/master/DNAnexus_and_AWS_data_structure.md)
 
 
## Meta data
 
The meta data proposal and specifications. Actual meta data is stored in [this repository](https://github.com/VGP/vgp-metadata).
* [Proposal](https://github.com/VGP/vgp-assembly/tree/master/metadata_proposal)
* [Specimen naming scheme](https://github.com/VGP/vgp-assembly/blob/master/VGP_specimen_naming_scheme.md)
 
 
## Citation
* VGP assemblies and genome assembly pipeline: Rhie et al., Towards complete and error-free genome assemblies of all vertebrate species, bioRxiv 2020. doi: https://doi.org/10.1101/2020.05.22.110833
 
* Mitochondrial genome assembly pipeline: Formenti et al., Complete vertebrate mitogenomes reveal widespread gene duplications and repeats, bioRxiv 2020. doi: https://doi.org/10.1101/2020.06.30.177956
