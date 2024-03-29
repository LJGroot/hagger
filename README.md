# hagger
#### L.J. Groot (l.j.groot@uva.nl)

## Contents of this repository
#### 1. General info
#### 2. Hagger_ML (data file, .sav)
#### 3. Hagger_MG (data file, .sav)
#### 4. Hagger_cor (data file, .Rdata)
#### 5. Hagger_n (vector, .rds file)
#### 6. Hagger_raw_unclusterd (.Rdata)
#### References

### 1. General info
This repository contains data (and, at some point, syntax) files generated for MASEM research, using `R`.
### 2. Hagger_ML (data file, .sav)
This file contains clustered data compiled from raw means reported in 39 datasets (n =  13185) in Hagger et al. (2022; see https://osf.io/3w2k7/), suitable for Multi-level Analysis. Import using `read_sav` function.
### 3. Hagger_MG (data file, .sav)
This file contains clustered data with 36 of 39 raw datasets (n = 10252) from Hagger_ML, suitable for Multi-Group Analysis (lower missingness). Import using `read_sav` function.
### 4. Hagger_cor (data file, .Rdata)
This .Rdata file contains an array of 39 correlation matrices computed from the raw data that were reported in Hagger et al. (2022), suitable for correlation based MASEM. Import with `readRDS` function [readRDS(gzcon(url("https://github.com/LJGroot/hagger/raw/main/Hagger_cor.Rdata")))]
### 5. Hagger_n (vector, .rds file)
This .rds file contains a vector of the sample sizes for the data that were reported in Hagger et al. (2022), to accompany the correlation matrices in Hagger_cor for correlation based MASEM using the `metaSEM` package. Import with `readRDS` function [readRDS(gzcon(url("https://github.com/LJGroot/hagger/raw/main/Hagger_n.rds")))]
### 6. Hagger_raw_unclustered (.Rdata)
This .Rdata file contains a workspace image of 39 seperate `n_obs` x 5 data frames for each of the studies reported on in Hagger et al. (2022). Essentially, these are cleaned up versions of the original files as they were published in the OSF repository, only containing the raw mean scores for 5 variables.
### References
Hagger, M. S., Cheung, M. W. -L., Ajzen, I., & Hamilton, K. (2022). Perceived behavioral control moderating effects in the theory of planned behavior: A meta-analysis. *Health Psychology*. Advance online publication. https://doi.org/10.1037/hea0001153
