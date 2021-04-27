# Accessibility-AccessRatios
Hi HUMAN!

These python codes are to calculate accessibility and access ratios based on the E2SFCA, M2SFCA, and 3SFCA methods.  
It could be seen as the very simple version of PySal. https://access.readthedocs.io/  
However, I did not succeed in installing the package. Rather, I found it is quite simple to calculate accessibility if you have the distance matrix between census tracts and facilities.

What is the meaning of "Accessibility" here ?  
Here, accessibility means the accessibility to public facilities.   
It is used to detect the distribution of public facilities, such as primary schools, hospitals, or even job opportunities.   
Using this indicator, we could identify which districts/areas in cities/regions has inferior provision of certain resource.

What is E2SFCA, M2SFCA, and 3SFCA method?  
FCA: floating catchment area method.  
FCA methods calculates accessibility of one population unit (such as a community, census block, or census tract) as the sum of supple-demand ratios of the facilities are nearby to the unit. The facilities are in the catchment (buffer zone) of the population unit, and the popluation unit is within the catchment of the facilities too.  
See detailed instruction: http://geodacenter.github.io/docs/PySALAccess%20Package_Documentation.pdf  

2SFCA: the two-step floating catchment area method.   
Luo, W., & Wang, F. (2003). Measures of spatial accessibility to health care in a GIS environment: synthesis and a case study in the Chicago Region. Environment and Planning B: Planning and Design, 30(6), 865-884. https://doi.org/10.1068/b29120 
E2SFCA: the enhanced two-step floating catchment area method.  
Luo, W., & Qi, Y. (2009). An enhanced two-step floating catchment area (E2SFCA) method for measuring spatial accessibility to primary care physicians. Health & Place, 15(4), 1100-1107. https://doi.org/10.1016/j.healthplace.2009.06.002
M2SFCA: the modiefied two-step floating catchment area method.  
Delamater, P. L. (2013). Spatial accessibility in suboptimally configured health care systems: a modified two-step floating catchment area (M2SFCA) metric. Health & Place, 24, 30-43. https://doi.org/10.1016/j.healthplace.2013.07.012  
3SFCA: the three-step floating catchment area method.  
Wan, N., Zou, B., & Sternberg, T. (2012). A three-step floating catchment area method for analyzing spatial access to health services. International Journal of Geographical Information Science, 26(6), 1073-1089. https://doi.org/10.1080/13658816.2011.624987  

What is access ratios?   
Access ratios = distance weights * Accessibility (for each paar of facility and cenesus tract).
According to Wan, Zhan, et al. (2012), access ratios can reduce the high sensitivity of the distance decay coefficient on accessibility results and can produce relatively stable accessibility results. However, there might be some limitations in certain conditions.
Wan, N., Zhan, F. B., Zou, B., & Chow, E. (2012). A relative spatial access assessment approach for analyzing potential spatial access to colorectal cancer services in Texas. Applied Geography, 32(2), 291-299. https://doi.org/10.1016/j.apgeog.2011.05.001 
