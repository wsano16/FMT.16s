# README
###### (updated December 6, 2018)

## FMT.16s: project repository for FISH546 Autumn 2018

***

### 1. General Description of your project including goals and objectives

   I began my project by doing microbiome analysis on 16S amplicons from Yue's Tibetan chiru fecal samples. The goal of this was to become familiar with the best practices of bioinformatics work and build an initial pipeline for later microbiome analyses.  
   
   My greater goal is to have my own data before the end of the quarter, which will be gut microbiome samples from African savannah, forest, and hybrid elephants spanning almost 20 years. The composition of these microbiomes has not been extensively studied, particularly in the case of hybrids. This study may yield greater insight into the gut microbial community of elephants and how it may vary continuously across hybrid zones.
   
   I did not generate these data in time for analysis in FISH546, so I have downloaded a published dataset on the microbiome of patients with _Clostridium difficile_ infections before and after fecal matter transplant vs. healthy controls. I used the pipeline I built around Yue's samples for these human samples, generating diversity analyses, and some intitial differential abundance plots.

### 2. A description of your repository structure, including what each directory includes, and describing any unique files.

  My repository includes the `FMT.16s.ipynb` Jupyter notebook, which contains the bulk of the code and visualizations that I made in this class. All scripts or text files for importing data are included in the `scripts` directory. `data` includes all raw and processed data, though raw data has not been pushed to GitHub.`analyses` includes all visualizations generated in QIIME2, which relies heavily on `.qzv` visualization files for data interpretation. 
  `wsano FISH546 Workflow.jpg` is a visual representation of my workflow, generation in draw.io

### 3. A projected timeline for project completion through week 10.

  *  **week 4:** ~~Complete sequence trimming(+), filtering(+), chimera checking (+), and pre-processing with Yue's data~~
  *  **week 5:** ~~Complete QIIME2 workflow with Yue's data(+), generating PCoA plots in Emperor(+). Start PERMANOVA testing(+). Differential abundance testing with Gneiss(+). Begin functional profiling with PICRUSt(+).~~
  *  **week 6:** ~~Finish functional profiling with PICRUSt.~~
  *  **week 7:** ~~Download and do partial run additional dataset to test ease of translation.~~
  *  **week 8:** ~~Set up mox account with HPC Club~~
  *  **week 9:** ~~Run second data set through mox, run elephant data (hopefully)~~
  *  **week 10:** Run FMT data, polish notebooks/repo for final submission
  
### 4. What is your question? 

         _Question 1_: Can I build a microbiome analysis pipeline that is easily extensible to new datasets?
         _Question 2_: How does the gut microbiome of patients with Clostridium difficile infections and ulcerative colitis change after fecal matter
         transplant relative to the microbiome of a healthy donor?
         
### 5. Process Visualization
         Flowchart data QIIME2 `provenance` function drawn up in draw.io, an online platform for creating workflow visualizations. Ths visualization will detail sequence preprocessing, filtering, ASV assignment in DADA2, and subsequent diversity, differential abundance, and functional profile analyses in QIIME2
         
         Visualization [here](https://github.com/wsano16/FMT.16s/blob/master/wsano%20FISH546%20Workflow.jpg)
         
### 6. End Products and Visualizations - contained withing FMT.16s.ipynb

          - taxa relative abundance barplots
          - summary barplots for each region
          - EMPeror plots to visualize beta diversity metrics (Bray Curtis, (Un)weighted UniFrac) by ASVs
          - Differential abundance plots
          - Summary PICRUSt output to communicate functional potential of sampled microbiomes
          
### 7. Next Steps
      Apply this same pipeline, which will hopefully recapitulate the analyses published in PMC5644368, to my elephant data.
