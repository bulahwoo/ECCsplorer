# Modified eccDNA-tools

This is a modified version of the [`ECCsplorer`](https://github.com/crimBubble/ECCsplorer) repository originally developed by [Mann et al. (2022)](https://doi.org/10.1186/s12859-021-04545-2).
All core functionality remains the same unless noted below. Please refer to the original repository for full documentation.

---

## Modifications in This Fork

1. Enhanced RepeatExplorer2 command in `config.py` to include additional options for logging and memory limits.
2. Added logging and memory options to RepeatExplorer2 execution in `eccClusterer.py`. This change enables automatic creation of a log file for RepeatExplorer2 execution (repex_log.txt) and control of the maximum memory usage (300,000,000 bytes, or ~300 MB).
3. Corrected ggplot2 y-aesthetic usage in `eccDNA_Rcodes.py` to ensures compatibility with ggplot2 versions ≥ 3.3.0 and improves code readability and makes aesthetics consistent across the plot.
4. Added debug logging for coverage calculations in `eccMapper.py` to captures the raw per-base coverage data for each region and mapping file. This helps track or reproduce specific failures or inconsistencies in the pipeline.
5. Added named CPU constants to `config.py` and applied named CPU constants in `eccMapper.py`. This enables adjustments to the number of parallel workers to prevent overloading the system or hitting OS limits.

---

## Original Repository

For detailed installation instructions, tool descriptions, and reference information, please visit the original repository:
[crimBubble/ECCsplorer](https://github.com/crimBubble/ECCsplorer).
