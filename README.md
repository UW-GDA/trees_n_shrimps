# trees_n_shrimps

Project Title:
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

## Conclusions and further direction

Overall, the code worked fairly well at achieving our goal. We switched from using Landsat to Sentinel-2 data, with a 10 meter resolution. We originally planned to clip our data by elevation and distance to coast, but didn't end up needing to do that. One challenge we ran into was harmonizing data over time, as Sentinel changed their data parameters in 2022 to allow negative reflectance, which impacted our CMRI analysis. 

We chose the Cà Mau peninsula because a group member had some familiarity with aquaculture in this region and we knew nearly all vegetation in this tile will be mangroves. In our analysis we encourtered both regrowth and reforestation by humans, and could oberve patterns of tree planting and cutting in the ponds. 

One struggle we ran into was with irregular pond shapes, which would also be an obstacle to expanding this program to analyze a larger and more diverse area. We also found there to be an ambiguous line between mangrove integrated and non-mangrove integrated ponds. 

Further directions to take this project in would be scaling up the program to be able to analyze larger and more varied areas, experimenting with the parameters of the segmentation to better show the ponds, and building a user interface for people to observe the data with. 

## Any other relevant information, images/tables, references, etc.

References

Ahn, H. K., Kwon, S., Song, C., & Lim, C.-H. (2025). Enhanced Rapid Mangrove Habitat Mapping Approach to Setting Protected Areas Using Satellite Indices and Deep Learning: A Case Study of the Solomon Islands. Remote Sensing, 17(14), 2512. https://doi.org/10.3390/rs17142512
Akbar, M. R., Arisanto, P. A. A., Sukirno, B. A., Merdeka, P. H., Priadhi, M. M., & Zallesa, S. (2020). Mangrove vegetation health index analysis by implementing NDVI (normalized difference vegetation index) classification method on sentinel-2 image data case study: Segara Anakan, Kabupaten Cilacap. IOP Conference Series: Earth and Environmental Science, 584, 012069. https://doi.org/10.1088/1755-1315/584/1/012069
American Museum of Natural History. (2024). The Importance of Mangrove Forests: Diverse Ecosystems | AMNH. American Museum of Natural History. https://www.amnh.org/explore/videos/biodiversity/mangroves/why-mangroves-matter
Geospatial School YouTube Channel- GEOBIA tutorial https://www.youtube.com/watch?v=hgmhERX4YBw
https://opensourceoptions.com/python-geographic-object-based-image-analysis-geobia/
Pimple et al. 2025. Tracking mangrove ecosystem dynamics: remote sensing approach for species classification and conservation assessment. Global Ecology and Conservation. doi.org/10.1016/j.gecco.2025.e03865
Gupta, K., Mukhopadhyay, A., Giri, S., Chanda, A., Datta Majumdar, S., Samanta, S., Mitra, D., Samal, R. N., Pattnaik, A. K., & Hazra, S. (2018). An index for discrimination of mangroves from non-mangroves using LANDSAT 8 OLI imagery. MethodsX, 5, 1129–1139. https://doi.org/10.1016/j.mex.2018.09.011
National Library of Medicine. (1994). The U.S. Military and the Herbicide Program in Vietnam. Nih.gov; National Academies Press (US). https://www.ncbi.nlm.nih.gov/books/NBK236347/
Python: Geographic Object-Based Image Analysis (GeOBIA) – Part 1: Image Segmentation – OpenSourceOptions. (2020, February 29). Opensourceoptions.com. https://opensourceoptions.com/python-geographic-object-based-image-analysis-geobia/
Ruan, L., Yan, M., Zhang, L., Fan, X., & Yang, H. (2022). Spatial-temporal NDVI pattern of global mangroves: A growing trend during 2000–2018. Science of the Total Environment, 844, 157075. https://doi.org/10.1016/j.scitotenv.2022.157075
Son, N.-T., Chen, C.-F., Chang, N.-B., Chen, C.-R., Chang, L.-Y., & Thanh, B.-X. (2015). Mangrove Mapping and Change Detection in Ca Mau Peninsula, Vietnam, Using Landsat Data and Object-Based Image Analysis. IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, 8(2), 503–510. https://doi.org/10.1109/JSTARS.2014.2360691
Vasquez et al. 2024. Determining Changes in Mangrove Cover Using Remote Sensing with Landsat Images: a Review. Water Air Soil Pollut, doi.org/10.1007/s11270-023-06788-6
Webb-Martin, S. (2022, May 24). NDVI IMPLICATIONS FOR MANGROVE HEALTH STUDIES. ArcGIS StoryMaps; Esri. https://storymaps.arcgis.com/stories/47d57669202f4aa38739a294747ea28f
