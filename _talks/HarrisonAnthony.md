---
name: 'Evaluating Microsatellite Instability Tools and Benchmarks'
speakers:
	- Harrison Anthony
categories:
	- Talk (8min)
---
Microsatellite instability (MSI) is a phenomenon seen in several cancer types that has been used as a biomarker for immune checkpoint inhibitor efficacy. With the advent of next-generation sequencing (NGS), researchers have created computational tools to categorize samples as MSI-high (MSI-H), MSI-low (MSI-L), or as being microsatellite stable (MSS). Most of these tools have been solely trained and tested on whole exome sequencing data (WXS) from The Cancer Genome Atlas (TCGA). This can be problematic as the tools were published with claims that they could be used with a variety of sequencing types, tumor purities, coverage thresholds, and, in some cases, without a matched normal sample. It raises the question of how useful these tools are for the task of classifying tumor samples using data from different platforms or in situations where a large set of normal samples is unavailable. We benchmarked several leading MSI tools on datasets resembling different sequencing scenarios. These included 10 random MSI-H, MSI-L, and MSS samples from TCGA whole genome sequencing (WGS) datasets; 20 random MSI-H, MSI-L, and MSS samples from TCGA WXS dataset; and 92 TSO-500 gene panel samples. We then used best practice settings for each tool to determine the MSI status for all samples. Precision, recall, and specificity were compared for all tools on each dataset. Early results suggest that the accuracy of MSI tools that do not require a matched normal sample is impacted by reducing the number of normal samples in the baseline, and we found a lack of concordance between tools trained on WXS data and the results of the TSO-500 pipeline. Concerningly, the accuracy of most tools was diminished on the WGS data, and there is some evidence that published AUC values might be inflated due to class imbalance in MSI data. Although most MSI tools claim accuracy close to 100%, we found discrepancies when testing them outside their optimal conditions and on different sequencing types.