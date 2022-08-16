# Requirements
The code was tested on python 3.10.4 with the following packages

scipy 1.9.0 

sklearn 1.1.2

numpy 1.23.1

pandas 1.4.3

matplotlib 3.5.2

swifter 1.3.3

prettytable 3.3.0 (to see lp results when verbose is turned on)

# Preprocessing

To download the original NYC taxi trip dataset, go to http://www.andresmh.com/nyctaxitrips/.
After the dataset is downloaded and unzipped, put the single csv file in the directory "/raw_data" (the experiment used "tripData2013/trip_data_1.csv" in the unzipped dataset, which is trip data of january 2013),
then run "nyc_data_analysis_and_process.ipynb" to process the dataset, the processed dataset will be named
"filtered_df.csv" located in "/filtered data". Because the dataset is large and the preprocessing steps can take 
some time, we have put the processed dataset in "/filtered data" already. But if you would like to go through
the preprocessing steps, simply follow the instructions above. 

# Implementation

"dependent_rounding.ipynb"      - implementation of the dependent rounding algorithm

"wrapper_classes.ipynb"         - implementation of driver and request objects

"algorithm_functions.ipynb"     - implementations of functions that set up the LP, functions that calculate objectives, and functions that run the algorithm repeatedly

NOTE: To optimize performance when running the experiments, some functions are implemented in an ad-hoc fashion
to support only two groups: advantaged and disadvantaged. If the current implementation were to be run with more than 
two groups, some appropriate modifications may be required. 

# Experiment

"figure1.ipynb" - Code to run the experiment that generated figure 1

"table1.ipynb" - Code to run the experiment that generated table 1

"appendix table.ipynb"  - Code to run the experiment that generated table in appendix



