# SPAT
### Surface Proteins Annotation Tool
#### Version 3 - updated April 2021

Annotation based on NextProt database:

* **Gold**: highest quality data, corresponding to error rates of <1%. 
* **Silver**: good quality data, corresponding to error rates of <5% (terms associated to the silver annotation are marked with an asterisk, ex: GO:0005887*) # not used for now

### AUTHOR

#### Jean-François Spinella, Ph.D. 
*jfspinella@gmail.com*

Team Dr. G.Sauvageau (Institute for Research in Immunology and Cancer, Université de Montréal, Canada)

### SYNOPSIS

`perl SPAT.v3.pl -help [brief help message] -man [full documentation]`

Annotation: `perl SPAT.v3.pl -input path/to/your/input/file.txt -format uniprot_id|ensembl_id|gene_name -output [path/to/your/output/directory/]`

### DESCRIPTION

* SPAT takes either uniprot_id, ensembl_id or gene_name as input in a .txt file and returns 1 SPAT score (and associated annotations)
* Scores and terms (CVTO, GO, SL) are updatable: update SPAT_scores.v3.txt file (be careful to conserve the original format)
* Please, don't modify files located in the SPAT/database directory

### DATE 

April 2021

### REQUIREMENTS

The following perl librairies must be installed: 

    -Array::Utils (installation: cpan Array::Utils)

    -Pod::Usage (installation: cpan Pod::Usage)

### OPTIONS

`-help <brief help message>`

`-man <full documentation>`

`-input <path/to/your/input/file.txt> mandatory`

`-format <uniprot_id|ensembl_id|gene_name> mandatory`

`-best_score <true|false> optional`

`-graph <true|false> optional`

`-score_threshold <0 to 1> optional`

`-output <path/to/your/output/directory/> optional`     
      
