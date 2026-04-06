**Phase 2: Differential Gene Expression (DGE) Analysis**
In this phase, the project moves from exploratory visualization to statistical significance testing. The goal is to identify which genes are mathematically "significant" regulators of the antiviral response.

**MethodologyStatistical Framework:** 
Modeled a DGE results object (Log2 Fold Change and p-values) to simulate a DESeq2 or edgeR output.
**Significance Thresholds:** 
**Fold Change:** $|Log2FC| > 1.0$ (representing a 2-fold change in expression).
**Statistical Power:** $p < 0.05$ (threshold for biological significance).
**Visualization:** Developed a publication-quality Volcano Plot using ggplot2 to map the relationship between effect size and statistical significance.

**Results Interpretation**
The Volcano Plot categorizes genes into three biological groups:
**UP-Regulated (Red):** Genes significantly induced by viral stress. These represent the primary antiviral effectors in the _B. mori_ immune system.
**DOWN-Regulated (Blue):** Genes significantly suppressed. These typically involve the downregulation of nutrient gatekeepers as the cell shifts resources to defense.
**Non-Significant (Black):** Genes whose expression changes were statistically negligible
**New Tools Used**
**Library:** ggplot2 (Data Visualization)
**Statistical Methods:** Log-transformation, P-value filtering, and Boolean categorization.
