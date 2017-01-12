# History of U.S. Energy Sources
This repository includes the sources, notes and methods for the data behind the graphics in Inside Energy's article and video, ["Energy Explained: Where Does It Come From And How Much Do We Use?"](LINKTK). There are two main data sets: per person energy use in the U.S., from 1790 to 2015, and the top fuel source for electricity generation by state, 2001 to 2015.


## Per Person Energy Use in the U.S., 1790 to 2015
The data used in our graphics is available to download in this repository in the file, *us-energy-use-1790-2015.csv*. The file contains the following fields:
* *Year*
* *Coal (Quadrillion Btu)*
* *Natural Gas (Quadrillion Btu)*
* *Petroleum (Quadrillion Btu)*
* *Hydro (Quadrillion Btu)*
* *Geothermal (Quadrillion Btu)*
* *Solar (Quadrillion Btu)*
* *Wind (Quadrillion Btu)*
* *Biomass (Quadrillion Btu)*
* *Total Primary Energy (Quadrillion Btu)*
* *Population*
* *Energy Per Capita (Btu)*

### Sources
Population data comes from the U.S. Census Bureau:
* [1970 to 1990, decadal count](U.S. Census Bureau - http://www.census.gov/population/www/censusdata/pop1790-1990.html)
* [1990 to 1999, annual estimates](https://www.census.gov/population/estimates/nation/popclockest.txt)
* [2000 to 2016, popuylation estimates](http://www.census.gov/data/tables/2016/demo/popest/nation-total.html)

Energy sources are from the U.S. Energy Information Administration and reflect primary energy use, by fuel type:
* [1790 to 1945](https://www.eia.gov/todayinenergy/detail.php?id=10)
* [1949 to 2009](https://www.eia.gov/totalenergy/data/browser/?tbl=T01.03#/?f=A&start=1949&end=2015&charted=1-2-3-5-12)
* [2009 to 2015](https://www.eia.gov/totalenergy/data/annual/archive/energyflow.php)

### Notes
Through 1945, the biomass column is exclusively wood. Post 1945, this includes all sources of biomass.

For time periods where energy sources and population were reported in alternating five-year intervals (i.e., energy data is from 1815, but population data is from 1820), we averaged the 1815 and 1825 energy totals to come up with an estimate for 1820.

## Top Electricity Source in Each State, 2001 to 2015
The data used to make maps for 2001, 2005, 2010 and 2015 top fuel source by state is available for download in the file, *top-fuel-2001-2005-2010-2015.csv*.

The raw data we used, from the EIA, is available in the file *Net_generation_for_all_sectors_2001_2015.csv*.

The script used to process and analyze the data is available as a Jupyter notebook, *state-electricity-generation-years.ipynb*.

### Sources
Data comes from the U.S. Energy Information Administration, downloaded from the [Electricity Data Browser](https://www.eia.gov/electricity/data/browser/#/topic/0?agg=2,0,1&fuel=vttb&geo=00fvvvvvvvvvo&sec=g&freq=A&start=2001&end=2015&ctype=linechart&ltype=pin&rtype=s&pin=&rse=0&maptype=0).

### Notes
Note that the EIA did not release information on distributed solar (i.e. rooftop solar) until 2014. We calculated the portion of electricity that came from each source using both the utility scale and the total (utility scale plus distributed solar, for 2015). In nearly every geography, the amount of distributed solar was negligible, to the extend that it didn't significantly change the overal electricity generation mix. Thus in the data file, the percent generated from each fuel source reflects utility scale values.

## Contact
For questions about this project, contact Jordan Wirfs-Brock, jordanwb at insideenergy dot org.