# 🗂️The datasets in this directory include: 

- **The initial Biginelli dataset**

A dataset comprising 4559 entries for 3869 unique Biginelli products. The file includes product and reactants structures, reaction yields, the information on the use of chromatographic purification. 

- **"FULL": the main curated dataset, used in this work**

3261 unique reaction records — 1722 “feasible” (with associated yields) and 1539 “non-feasible” (yield assumed zero). The yields of repeated entries were averaged. 

- **“ALT+”**
  
In the dataset, there were instances of reactions showing different regioselectivity. Hypothesizing that in each such case the alternative regioisomer is not formed at all, these alternative products were added to the dataset with a yield of zero. 

- **“YMAX”**

It might be assumed that in the case of repeated experiments, the best outcome is the best estimate of chemical reactivity and lower yields are probably due to experimental mistakes. The "YMAX" dataset was generated from the initial dataset by keeping the highest reported yield in case of repeated reactions.

- **“B&W”**

“B&W” version of the training set was also used for classification models, obtained by eliminating reactions with yields >0 but <20% from “FULL”.

- **“FULL-OF”**

Some outliers were detected at the model-building stage. “FULL-OF” refers to the "FULL" dataset with 446 such outliers removed. 

- **“VAL”**

The models built on the initial dataset were applied to the external validation set “VAL” containing 476 reactions.


### 🔍For more information about the datasets and data curation protocols, please refer to the [paper](https://chemrxiv.org/doi/full/10.26434/chemrxiv.15000783/v1) and its Supplementary Information. 
