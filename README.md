# Modified ECCsplorer

This is a modified version of the [`ECCsplorer`](https://github.com/crimBubble/ECCsplorer) repository originally developed by [Mann et al. (2022)](https://doi.org/10.1186/s12859-021-04545-2).  
All core functionality remains the same unless noted below. Please refer to the original repository for full documentation.

---

## Modifications in This Fork

1. Enhanced the RepeatExplorer2 command in `config.py` to include additional options for logging and memory limits.  
2. Added logging and memory options to RepeatExplorer2 execution in `eccClusterer.py`, enabling automatic creation of a log file (`repex_log.txt`) and control over maximum memory usage (~300 MB).  
3. Corrected {ggplot2} y-aesthetic usage in `eccDNA_Rcodes.py` to ensure compatibility with {ggplot2} ≥ 3.3.0, improving code readability and aesthetic consistency across plots.  
4. Added debug logging for coverage calculations in `eccMapper.py` to capture raw per-base coverage data for each region and mapping file. This aids troubleshooting and reproducibility.  
5. Introduced named CPU constants in `config.py` and applied them in `eccMapper.py` to allow easy adjustment of parallel worker counts, helping prevent system overload and multiprocessing issues.

---

## Original Repository

For detailed installation instructions, tool descriptions, and reference information, please visit the original repository:  
[crimBubble/ECCsplorer](https://github.com/crimBubble/ECCsplorer).
