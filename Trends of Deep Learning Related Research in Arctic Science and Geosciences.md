# Trends of Deep Learning Related Research in Arctic Science and Geosciences

## 1. Goal

The goal of this research is to reveal recent trends of publications that uses advanced **AI-driven analytics**, particularly deep learning technology, to support research in Arctic science and other geoscience domains. We reviewed 232 geoscience journals and use search terms "deep learning" with and without "Arctic" to find relevant articles from 2015-2021. Google scholar API is leveraged for conducting automated search. The results are analyzed and manually checked to remove duplications and other uncertainties. 

## 2. Method

### 2.1 Identify geoscience related journals

To produce more accurate statistics of the AI-based research trends in Arctic science specifically and geoscience in general, and to reduce the uncessary search in journals that may be less likely to contain AI related technical research, we introduced a strategy to narrow down the research scope (journals) by selecting geoscience journals that may have a technical focus, rather than iterating all the journals or articles in geoscience/environmental science domains. Specifically, we referred to a comprehensive review paper ([Reichstein et al., 2019](#ref1)) that summarizes the recent research adopting deep learning in Earth System Science research. Starting from the journals listed in the reference of the paper [^1], we further expanded the journal list by exploiting a journal ranking database [Scimagojr](https://www.scimagojr.com/journalrank.php), with the following steps:

1.	Find all subject categories in database Scimagojr that cover the journals[^1] referred by the review paper. Based on this search, we were able to select the following subject categories shown in [Appendix A-1](#apdx1). 
2.	For each subject category, find out all the journals that have an impact factor higher than 1 (SJR > 1). 
3.	Merge all the collected journals from each subject category and remove any duplications. 

We finally retrieved 232 journals from the above steps. See a full list of the journals in [Appendix A-2](#apdx2).

### 2.2 Retrieve and count papers published with and without an Arctic focus

With Google Scholar API, and by specifying the keyword ("deep learning" + "Arctic" or "deep learning"), journal name, and publication year (see [sample query](#sample_q) below), we were able to retrieve the number of articles published in each selected journal from 2015 to 2021. Based on this information, we further produced the statistical chart that present the trends of research in Arctic Science and the rest of Geoscience domains that use AI and deep learning. 

[^1]: we manually selected the journals that are relevant to earth science or geoscience.

<a name="sample_q"></a>
#### A Sample Query
```
https:/scholar.google.com/scholar?
as_q="deep learning" "arctic"&
as_publication="Remote Sensing of Environment"&
as_ylo=2021&as_yhi=2021&hl=en-US
```
After URL encoding, the query is finally formatted as follows:
```
https:/scholar.google.com/scholar?as_q=%22deep%20learning%22%20%22arctic%22&as_publication=%22Remote%20Sensing%20of%20Environment%22&as_ylo=2021&as_yhi=2021&hl=en-US
```

## 3. Results

Using the keyword "deep learning", we obtain the trend of utilizing deep learning in geoscience research, the numbers are in column "**Papers using 'deep learning' in the geoscience domains**". Similarly, we obtain the numbers in column "**Arctic science papers that use 'deep learning'**" using keywords "deep learning"+"arctic". By calculating the difference between the above two columns, we obtained the number in column "**Other geoscience papers that use 'deep learning'**". We found in the results that the AI and deep learning related papers are highly clustered in journals that have a remote sensing focus (e.g., Remote Sensing of Environment, IEEE Transactions on Geoscience and Remote Sensing) or a domain foccus (e.g., Journal of Climate, Geophysics, Geophysics Research Letters, Cryosphere). To improve the results accuracy, we manually checked results from these journals to remove duplications and irrelvant results. The final results can be found in [figure 1](#fig1).

<a name="fig1"></a>
![trend](images/fig1.png)
_Figure 1. Trends of deep learning related research in arctic science and geosciences during 2015-2021_  
<br/>

## 4. Potential issues and uncertainties

In this research, although we developed several quality-control mechanisms, such as (1) refining the research scope (to focus on more technical journals), (2) adopting very specific keywords while performing the search, and (3) manually checking results from several journals that have a high number of returned publications, the results may still have sone uncertainties and some degree of errors because of the very large volume of total returned results. For example, articles that only mention "deep learning" in the main text (our search does not consider "Reference" section of the paper) but not directly apply "deep learning" may still be considered relevant in our results. Thus, the produced statistics might be a little higher than it should be. However, the trends on arctic science and geoscience are still valid to be compared, supposing they share the similar uncertainty rate. 

## References
<a name="ref1"></a>Reichstein, M., Camps-Valls, G., Stevens, B., Jung, M., Denzler, J., & Carvalhais, N. (2019). Deep learning and process understanding for data-driven Earth system science. *Nature, 566(7743)*, 195-204.

## Appendix

<a name="apdx1"></a>
### A-1. Selected Subject Category list in [Scimagojr](https://www.scimagojr.com/journalrank.php)

Atmospheric Science  
Computers in Earth Sciences  
Earth and Planetary Sciences (miscellaneous)  
Earth-Surface Processes  
Environmental Science (miscellaneous)  
Geography, Planning and Development  
Geophysics  

<a name="apdx2"></a>
### A-2. Full Journal List
AAPG Bulletin  
Acta Geotechnica  
Advanced Sustainable Systems  
Advances in Atmospheric Sciences  
Advances in Climate Change Research  
Aeolian Research  
African Affairs  
Agricultural and Forest Meteorology  
Agricultural Water Management  
Ambio  
American Journal of Science  
American Mineralogist  
Annals of the American Association of Geographers  
Anthropocene  
Antipode  
Applied Catalysis B: Environmental  
Applied Geography  
Aquaculture, Economics and Management  
Atmospheric Chemistry and Physics  
Atmospheric Environment  
Atmospheric Environment: X  
Atmospheric Measurement Techniques  
Atmospheric Research  
Big Earth Data  
Biogeochemistry  
Biogeosciences  
BMC Ecology  
Boundary-Layer Meteorology  
Building and Environment  
Bulletin of Earthquake Engineering  
Bulletin of the American Meteorological Society  
Bulletin of the Seismological Society of America  
Business Strategy and the Environment  
Cambridge Journal of Regions, Economy and Society  
Capitalism, Nature, Socialism  
Carbon Balance and Management  
Catena  
China Journal  
China Quarterly  
City  
Climate and Development  
Climate Dynamics  
Climate Policy  
Climate Risk Management  
Climate Services  
Climatic Change  
Cold Regions Science and Technology  
Computers, Environment and Urban Systems  
Contributions to Mineralogy and Petrology  
Cryosphere  
Current Climate Change Reports  
Current Issues in Tourism  
Current Opinion in Environmental Sustainability  
Democratization  
Dialogues in Human Geography  
Earth and Planetary Science Letters  
Earth Interactions  
Earth Surface Dynamics  
Earth Surface Processes and Landforms  
Earth System Dynamics  
Earth System Science Data  
Earth-Science Reviews  
Earth's Future  
Earthquake Engineering and Structural Dynamics  
Earthquake Spectra  
Ecological Economics  
Economic Geography  
Economic Geology  
Ecosystem Services  
Egyptian Journal of Remote Sensing and Space Science  
Elementa  
Elements  
Energy for Sustainable Development  
Environment and Behavior  
Environment and Planning A  
Environment and Planning C: Politics and Space  
Environment and Planning D: Society and Space  
Environment and Society: Advances in Research  
Environment and Urbanization  
Environmental Impact Assessment Review  
Environmental Innovation and Societal Transitions  
Environmental International  
Environmental Politics  
Environmental Research  
Environmental Research Letters  
Environmental Reviews  
Environmental Science and Policy  
Environmental Science: Nano  
European Planning Studies  
European Urban and Regional Studies  
Frontiers in Earth Science  
Frontiers in Environmental Science  
Frontiers in Marine Science  
Geobiology  
Geochemistry, Geophysics, Geosystems  
Geographical Journal  
Geography Compass  
Geomorphology  
Geophysical Journal International  
Geophysical Research Letters  
Geophysics  
Geoscience Frontiers  
Geoscience Letters  
Geoscientific Model Development  
Geotechnique  
GIScience and Remote Sensing  
Global Biogeochemical Cycles  
Global Change Biology  
Global Environmental Change  
GPS Solutions  
Groundwater for Sustainable Development  
Health and Place  
Holocene  
Hydrology and Earth System Sciences  
IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing  
IEEE Transactions on Geoscience and Remote Sensing  
International Journal of Applied Earth Observation and Geoinformation  
International Journal of Climatology  
International Journal of Earth Sciences  
International Journal of Geographical Information Science  
International Journal of Housing Policy  
International Journal of Life Cycle Assessment  
International Journal of Sustainable Transportation  
International Journal of Tourism Research  
Island Studies Journal  
ISPRS Journal of Photogrammetry and Remote Sensing  
Journal of Advances in Modeling Earth Systems  
Journal of African Business  
Journal of Applied Meteorology and Climatology  
Journal of Applied Volcanology  
Journal of Asian Earth Sciences  
Journal of Cleaner Production  
Journal of Climate  
Journal of Economic Geography  
Journal of Environmental Education  
Journal of Environmental Informatics  
Journal of Environmental Sciences  
Journal of Flood Risk Management  
Journal of Geodesy  
Journal of Geographical Sciences  
Journal of Geophysical Research  
Journal of Geophysical Research: Solid Earth  
Journal of Geotechnical and Geoenvironmental Engineering - ASCE  
Journal of Glaciology  
Journal of Hydrology: Regional Studies  
Journal of Hydrometeorology  
Journal of Industrial Ecology  
Journal of Petrology  
Journal of Planning Literature  
Journal of Quaternary Science  
Journal of Regional Science  
Journal of Rural Studies  
Journal of Space Weather and Space Climate  
Journal of Sustainable Tourism  
Journal of the American Planning Association  
Journal of Transport and Land Use  
Journal of Transport Geography  
Journal of Travel Research  
Journal of Volcanology and Geothermal Research  
Journals of the Atmospheric Sciences  
Land Degradation and Development  
Land Use Policy  
Landscape Ecology  
Long Range Planning  
Marine and Petroleum Geology  
Marine Policy  
Maritime Policy and Management  
Meteoritics and Planetary Science  
Meteorological Monographs  
Mineralium Deposita  
Mobilities  
Monthly Weather Review  
Natural Hazards and Earth System Sciences  
Nature Climate Change  
Nature Geoscience  
Nature Sustainability  
New Political Economy  
npj Climate and Atmospheric Science  
Ocean Modelling  
Organization and Environment  
Palaeogeography, Palaeoclimatology, Palaeoecology  
Paleoceanography and Paleoclimatology  
Physics of the Earth and Planetary Interiors  
Planning Theory  
Planning Theory and Practice  
Political Geography  
Population and Environment  
Population, Space and Place  
Proceedings of the Royal Society B: Biological Sciences  
Progress in Earth and Planetary Science  
Progress in Human Geography  
Progress in Physical Geography  
Progress in Planning  
Quarterly Journal of the Royal Meteorological Society  
Quaternary Geochronology  
Radiocarbon  
Regional Studies  
Remote Sensing  
Remote Sensing in Ecology and Conservation  
Remote Sensing of Environment  
Reviews of Geophysics  
Science China Earth Sciences  
Science China Life Sciences  
Scientific Online Letters on the Atmosphere  
Seismological Research Letters  
Social and Cultural Geography  
Socio-Economic Planning Sciences  
Soil and Tillage Research  
Solid Earth  
Space Weather  
Surveys in Geophysics  
Sustainability Science  
Sustainable Cities and Society  
Tectonics  
Tectonophysics  
Tellus, Series A: Dynamic Meteorology and Oceanography  
Tourism Geographies  
Tourism Review  
Transactions of the Institute of British Geographers  
Transport Policy  
Transportation Research, Part D: Transport and Environment  
Urban Climate  
Urban Geography  
Urban Studies  
Water Resources and Industry  
Water Resources and Rural Development  
Weather and Climate Extremes  
Weather and Forecasting  
Weather, Climate, and Society  
Wiley Interdisciplinary Reviews: Climate Change  
Wiley Interdisciplinary Reviews: Energy and Environment  
World Development  
