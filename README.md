# CMDIF Method
A framework for extracting surface water using collaborative optical and SAR images.Here we present the sample code of CMDIF, including registration of different data sources, water body extraction from Sentinel-2 images, water body extraction from Sentinel-1 images, as well as the complete process of CMDIF. Due to the computing power limitations of the GEE platform, we use a part of Kyoga Lake as an example for demonstration. During the actual process, we adopt a phased data processing approach for large-scale water system mapping, that is, each part of the data processing is downloaded to the local area for parameter evaluation, data fusion, etc. The provided code also includes the main functions implemented in this study, which can provide certain references for researchers.All the codes are written using JavaScript scripts. Researchers can simply copy them and view them on the GEE platform.


# CMDIF_data registration
We demonstrated using the public dataset registration data from 2021, integrating the resolutions and geographic coordinates of multiple data sources.

# CMDIF_S1
This code demonstrates the Edge-otsu water body extraction algorithm processed based on SNIC.

# CMDIF_S2
This code demonstrates the process of water body extraction using Sentinel-2, including dataset resampling, sample generation, random forest classification. Since the layer overlay of multi-source datasets is operated locally, here we use the Dynamic World dataset as an example for demonstration. This dataset can be called in GEE and can provide example data for researchers to understand the method of this study.

# CMDIF
This code integrates four stages: Sentinel-1 water body extraction, Sentinel-2 water body extraction, hierarchical decision fusion, and post-processing. It operates using multiple data sets and constitutes a complete CMDIF water body extraction framework.
