The Jupyter Notebooks in this directory are made by
Griffon Hoeven for sharing of Python code techniques
and notes.

The links below are to static renderings of the notebooks via
[nbviewer.org](https://nbviewer.org/).
Descriptions below the links are from the first cell of the notebooks
(if that cell contains Markdown or raw text).

* ## [wm_divide.ipynb](https://nbviewer.org/github/SalishSeaCast/analysis-griffon/blob/main/notebooks/wm_divide.ipynb)  
    
    **divide observations into watermasses based on location**


## ---------------------
## DATA & FILE OVERVIEW
## ---------------------

File List:

File: wm_divide.ipynb
Short description: Initial draft file I was given for seperating watermasses in CCS

Folder: CaliforniaCurrentAnalysis  
Description: Data processing and analysis for the CCS
1. File: myobs.ipynb  
Description: Originally given from bbeutel for processing raw data from various datasets. Added CalCOFI dataset to it. It outputs the PNW_obs_compiled.csv file which is a dataframe of all of the various data compiled together.
2. File: DefiningCurrentRegions.ipynb  
Description: Long file containing breakdown into the 3 different water masses based on various definitions we used. It also contains many exploratory plots that helped understand some properties of the currents. It takes the dataframe from myobs.ipynb and returns a dataframe with additional columns for the current the datapoint belongs to. This dataframe is stored as PNWCurrent_obs.csv
3. Files: CurrentAnalysis_*  
Description: Each of these files contains specific figures I made to summarize properties in the 3 watermasses. These contain things like property trends, rates up and down the currents, temporal data density etc. This takes the dataframe with currents defined in DefiningCurrentRegions.ipynb
4. File: InitialObsPlotting*  
Description: These two files are largely the same and just had some exploratory figures looking at the profiles and data we first got from myobs.ipynb.
5. File: PreliminaryCurrentAnalysis.ipynb   
Description: After seperating the currents, this was my first attempt at plotting the properties. Contained in here are some plots of spatial and temporal data density and then anomaly plots compared with climate indicators ENSO, NPGO, PDO. The sources for these indicators are in this notebook

Folder: ArianeResidenceTime  
Description: Notebooks for understanding Ariane output and calculating residence times.
1. File: TracerResTime.ipynb  
Description: This was the final draft of the filtering methods and what can be used to filter runs with tracers included. This is the main script to run to get residence time results.
2. File: SensitivityAnalysis.ipynb  
Description: Plots of the sensitivity analysis when different filters are employed.
3. File: MapBoundaries.ipynb  
Description: Shows the grid/map for puget sound and boundaries that were used for the QNT runs in Ariane
4. File: QualitiativePlotting.ipynb  
Description: Plotting spaghetti plots for the sample qualitative runs I ran along with depth trajectories
5. File: PennCovePlot.ipynb  
Description: First exploratory analysis of QNT output from Penn Cove, Holmes Harbour, Lynch Cove, etc. It shows histograms, filters and 2d histograms of initial positions vs final positions. Also stats are calculated for each inlet
6. File: QualLatLonConversionAndEddyError.ipynb  
Description: Some experiementation with conversion between grid coordinates and lat, lon. Also, plotting for eddy errors and coast crash errors with the velocity fields at the points.
7. Files: RegionResTimePlotting*  
Description: Notebooks for calculating residence time with depth filters, these were used before I had the analysis script which is TracerResTime.
8. File: TwoBoundaryCove.ipynb  
Description: Experimenting with residence time calculations in multiple boundary regions (ex. putting a second boundary within an inlet)
      
## License

These notebooks and files are copyright by the
[UBC EOAS MOAD Group](https://github.com/UBC-MOAD/docs/blob/main/CONTRIBUTORS.rst)
and The University of British Columbia.

They are licensed under the Apache License, Version 2.0.
http://www.apache.org/licenses/LICENSE-2.0
Please see the LICENSE file in this repository for details of the license.
