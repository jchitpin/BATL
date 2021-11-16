# BATL - Bayesian annotations for targeted lipidomics

Bioinformatic tools capable of annotating, rapidly and reproducibly, large, targeted lipidomic datasets are limited. Specifically, few programs enable high-throughput peak assessment of liquid chromatography-electrospray ionization tandem mass spectrometry (LC-ESI-MS/MS) data acquired in either selected or multiple reaction monitoring (SRM and MRM) modes. We present here Bayesian Annotations for Targeted Lipidomics (BATL), a Gaussian naïve Bayes classifier for targeted lipidomics that annotates peak identities according to eight features related to retention time, intensity, and peak shape. Lipid identification is achieved by modelling distributions of these eight input features across biological conditions and maximizing the joint posterior probabilities of all peak identities at a given transition. When applied to sphingolipid and glycerophosphocholine SRM datasets, we demonstrate over 95% of all peaks are rapidly and correctly identified.


## Web server for BATL

A graphical user interface version of BATL is available at http://complimet.ca:3838/batl/ or http://complimet.ca/batl/

## Installation

BATL requires R, (RStudio optional but recommended), and relies on several mandatory R packages.

1. R version 3.6.0 or greater required and RStudio IDE.
2. Download latest BATL tar.gz file (Code -> Download ZIP is the easiest way)
3. In RStudio console: `install.packages(c("data.table", "doFuture", "future", "foreach", "igraph", "openxlsx", "progressr))`
4. In RStudio top menu bar:
  * Tools -> Install Packages...
  * Install from: Package Archive File (.tar.gz)
  * Package archive: Browse -> Select batl_X.XX.X.tar.gz
  * Red text in the console will indicate successful installation ending with `DONE (batl)`   

## Usage

Function descriptions and usage are found in the accompanying vignette.

* In RStudio console: `vignette(package = "batl", topic = "batl-Introduction")`

## Citation

Chitpin JG, Surendra A, Nguyen TT, Taylor GP, Xu H, Alecu I, Ortega R, Tomlinson JJ, Crawley AM, McGuinty M, Schlossmacher MG, Saunders-Pullman R, *Cuperlovic-Culf M, *Bennett SAL *Perkins TJ,(2021) BATL: Bayesian annotations for targeted lipidomics.
bioRxiv. [doi.org/10.1101/2021.03.18.435788](doi.org/10.1101/2021.03.18.435788).

