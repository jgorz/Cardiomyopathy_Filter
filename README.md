# Cardiomyopathy_Filter
AIM: Filter annotated variant call files (in form of .txt) for variants who reach specified quality threshold in genes associated with human cardiomyopathy/cardiovascular disease.

Written in BASH


Require inputs:

  Line 2, path to annotated variant call (.txt) file.  NOTE: in order for the quality filter to work, the quality score must be in column 5
  Line 3, sample name-- this will also be incorporated into the output file names
  Line 4, minimum qulaity score threshold (numeric)
  
  Outputs: 
  Directory: 
    Parent: $Sample"_minQAUL_"$Min_QUAL
      sub: directory for each cardiomyopathy (DCM, HCM, ARVC) with .txt files for all variants and for only exonic variants
