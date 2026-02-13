# trees_n_shrimps

Project Title
Remote Sensing of Mangrove Change 

Name(s) of individual or team members
Will Burnham, Nick Giovine, Zeke Cohn
See requirement above for at least one contribution/commit from each team member on the project README.md. Adding names is a good way to practice collaboratively editing a file on Github.

Short 1-2 sentence summary
The goal of this project is to develop tools which can be used to quickly generate maps documenting historic mangrove change, both in terms of area/conversion and qualitatively through various vegetation indices, using Landsat imagery.
Some introductory background information
Mangroves forests, composed of several families of trees and shrubs inhabiting tropical intertidal wetlands, provide a wide range of ecosystem services, including enhanced protection from storm surges, fish nursery provision, and high carbon storage volumes. However, global mangrove extent has declined significantly since the mid 20th century, driven by factors such as coastal urban development, deforestation for fuelwood and, most notably, the expansion of shrimp aquaculture. Establishing historical mangrove extent/quality is essential for understanding mangrove loss dynamics and prioritizing target areas for restoration/rehabilitation. We will aim to monitor changes from the 70s to the present, based on availablity of Landsat images.

Problem statement, question(s) and/or objective(s)
Gain familiarity with using Landsat imagery to map mangroves
Create tools which can easily be applied to new AOIs

Datasets you will use (with links, if available)
Landsat imagery https://www.usgs.gov/landsat-missions/landsat-data-access

Tools/packages you’ll use (with links)
Holoviews: https://holoviews.org/getting_started/index.html 
Panel: https://panel.holoviz.org/getting_started/index.html 
Packages from class: matplotlib, numpy, pandas, geopandas, contextily

Planned methodology/approach
Download cloud-free images of target area within desired time range
Clip to coastal buffer, filter to low-elevation (SRTM?)
Supervised ML classification
Calculate area statistics, map NDVI, MVI in mangrove areas
Expected outcomes
Time series and table of mangrove area change, LULC conversion matrix 
GIF of mangrove area change
Possibly try to create a simple interface in Holoviews or Panel

Any other relevant information, images/tables, references, etc.
References
Pimple et al. 2025. Tracking mangrove ecosystem dynamics: remote sensing approach for species classification and conservation assessment. Global Ecology and Conservation. doi.org/10.1016/j.gecco.2025.e03865
Vasquez et al. 2024. Determining Changes in Mangrove Cover Using Remote Sensing with Landsat Images: a Review. Water Air Soil Pollut, doi.org/10.1007/s11270-023-06788-6


Quinn’s comments:
“Sounds great! Quantifying decreases in mangrove area should be straightforward with Sentinel-2, Landsat, or harmonized Landsat Sentinel-2 (HLS, https://planetarycomputer.microsoft.com/dataset/storage/hls) and NDVI or MVI. You'll potentially want to explore NDVI change detection. Consider--on what time scale do you expect to see change, and on what time scale is it relevant to measure change (Since the 1980s? Since 2020?). That will help you pick your datasets. 
As for the interface, consider Holoviews (https://holoviews.org/gallery/) and Panel (https://panel.holoviz.org/gallery/index.html) to make a lightweight app.”
