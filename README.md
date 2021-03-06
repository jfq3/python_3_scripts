# python_3_scripts
The python scripts in RDPTools and FunGene Pipeline are written in python 2. If you are not able to run these programs because you have only python 3 installed, you may substitute the python scripts in RDPTools and FunGene_Pipeline with the python 3 scripts in this repository. The locations for the scripts are:
## RDPTools  
/path/to/RDPTools/Clustering/mcupgma.py  
/path/to/RDPTools/AlignmentTools/parseErrorAnalysis.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/estimate_optimal_with_N_and_M.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/getUniqueStarts.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/compareOpennodes.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/randomSelectKmer.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/fetch_ncbi_xml.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/mergeTaxonAbund.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/compareOpennodesTwodirection.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/mergeNearstmatchAbund.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/reverse.py  
/path/to/RDPTools/Xander_assembler/pythonscripts/parse_ncbi_lineage.py  

## Possible edits to RDPTools bash script files  
Download the test file hello.py, make sure it is executable, and attempt to run it with:  

python hello.py  

If you get an error, then try:  

python3 hello.py  

If that works, then edit lines beginning with python in the following files to begin with python3 instead:  

/path/to/RDPTools/Xander_assembler/bin/run_xander_findStarts.sh:  
python3 ${REF_DIR}/pythonscripts/getUniqueStarts.py temp_starts_*.txt > uniq_starts.txt; rm temp_starts_*.txt  

/path/to/RDPTools/Xander_assembler/bin/prepare_gene_ref.sh:  
python3 ${JAR_DIR}/Xander_assembler/pythonscripts/reverse.py ${gene}_seeds_aligned.fasta  

## FunGene_Pipeline  
/path/to/fungene_pipeline/fgp_wrapper.py  
/path/to/fungene_pipeline/seq_trimmer_model.py  
/path/to/fungene_pipeline/pipeline_core.py  
/path/to/fungene_pipeline/titanium_options.py  
/path/to/fungene_pipeline/pipeline.py  
/path/to/fungene_pipeline/parseErrorAnalysis.py  
/path/to/fungene_pipeline/titanium_run_processor.py  

