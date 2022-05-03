# Zero-Till Effects on WHC in Spain
Applies empirical statistics of zero-tillage enhancement upon conventionally farmed land to see the potential benefits (in the form of increased soil water retention) after conversion to a regenerative farming methods.

Repo use:

The file <Greig_Project.ipynb> contains the script and model that projects soil water holding.

All the other files (sans standard git/git hub files) contain data necessary for the script. Due to some datas' file size, they have not been pushed to this repo. Please see the following web addresses to get other necessary data. Also, all files were taken out of their hierarchical directory during the project, so please be sure to amend paths for the data when running the script (all file names are consistent though).

Spain Boundary shape file: https://international.ipums.org/international/gis.shtml
European top soil bulk density raster:https://esdac.jrc.ec.europa.eu/content/european-soil-database-derived-data
WHC raster: https://www.nrcs.usda.gov/wps/portal/nrcs/detail/soils/use/worldsoils/?cid=nrcs142p2_054022

Model framework:

Apply zero-tillage potential to large-scale area.
On lands currently conventionally tilled, increase whc by a factor derived from field studies on zero-tillage's effect on whc in Spanish soils. Calculate the difference in whc after applying the zero-tillage factor and multiply by the surface area over which difference applies (conventionally tilled land). Multiply difference-volume by soil pore space (ascertained by bulk density and particle density) to reflect potential soil water holding increases. Projection intervals/ranges constructed from minimum whc, average whc, and max whc of ranges provided in data.

Limitations:

Projection represents saturated soil water holding, not elevated field capacity. Zero-tillage statistic taken from limited studies without variability estimates. WHC within top 30cm of soils only. WHC and agricultural data lack accuracy and granularity, wide ranges used to construct projected intervals.
