# trees_n_shrimps

Project Title
Remote Sensing of Mangrove Change 

## Name(s) of individual or team members

Will Burnham, Nick Giovine, Zeke Cohn

## Short 1-2 sentence summary

The goal of this project is to develop a workflow to classify change in mangrove and silvofisheries areas using Object-Based Image Analysis with Sentinel-2 imagery.

## Some introductory background information

Mangroves forests, composed of several families of trees and shrubs inhabiting tropical intertidal wetlands, provide a wide range of ecosystem services, including enhanced protection from storm surges, fish nursery provision, and high carbon storage volumes. However, global mangrove extent has declined significantly since the mid 20th century, driven by factors such as coastal urban development, deforestation for fuelwood and, most notably, the expansion of shrimp aquaculture. Many models of shrimp aquaculture exist, including some which integrate mangrove trees into the design of the pond, so called "silvofisheries" or integrated-mangrove pond models. This project aims to use Object-Based Image Analysis to map mangrove and integrated-mangrove aquaculture change in southern Vietnam, using Sentinel-2 images from 2017 and 2026.

## Problem statement, question(s) and/or objective(s)
Gain familiarity with using Sentinel imagery to map mangroves
Test the applicability of bject-based image analysis to mangrove areas, especilaly for shrimp ponds in former mangrove areas
Calcualte basic change statistics 
Create tools which could be applied to new AOIs

## Datasets you will use (with links, if available)

https://planetarycomputer.microsoft.com/dataset/sentinel-2-l2a

## Tools/packages you’ll use (with links)

skimage: https://scikit-image.org/
sklearn: https://scikit-learn.org/stable/
Packages from class: matplotlib, numpy, pandas, geopandas, seaborn, gdal, xarray, rioxarray, rasterio

## Planned methodology/approach

Download cloud-free images of target area within desired time range
Create indices
Calculate area statistics, map NDVI, CRMI, NDWI in mangrove areas
Create training data in QGIS
Complete OBIA proess: segmentation, classification
Analyze- confusion matrix, accuracy

## Any other relevant information, images/tables, references, etc.

References
Geospatial School YouTube Channel- GEOBIA tutorial https://www.youtube.com/watch?v=hgmhERX4YBw
https://opensourceoptions.com/python-geographic-object-based-image-analysis-geobia/
Pimple et al. 2025. Tracking mangrove ecosystem dynamics: remote sensing approach for species classification and conservation assessment. Global Ecology and Conservation. doi.org/10.1016/j.gecco.2025.e03865
Vasquez et al. 2024. Determining Changes in Mangrove Cover Using Remote Sensing with Landsat Images: a Review. Water Air Soil Pollut, doi.org/10.1007/s11270-023-06788-6
Nguyen et al. 2015. Mangrove Mapping and Change Detection in Ca Mau Peninsula, Vietnam, Using Landsat Data and Object-Based Image Analysis. IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, 8(2) 10.1109/JSTARS.2014.2360691
M R Akbar et al. 2020. Mangrove vegetation health index analysis by implementing NDVI (normalized difference vegetation index) classification method on sentinel-2 image data case study: Segara Anakan, Kabupaten Cilacap. IOP Conf. Ser.: Earth Environ. Sci. 584 012069



