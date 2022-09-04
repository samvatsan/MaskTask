# MaskTask

## Parts of the Program
(The code may be out of order as it was imported from multiple files)

1. Raw Mask Data Generator (generation of random numbers based on Gaussian Distribution—around a mean and standard deviation—to model data that the program would get from the iButton Hygrochron sensor)
	a. This program is located toward the end of the code, and is marked by a text block

2. Generated data used in determining whether mask is on or off
	a. This is located right above the random generation code**, and uses a threshold value for temperature and relative humidity within a mask (data given by the random generation function) in order to determine when a mask is on or off, and list the values when it is on

3. Calculate the number of hours the mask is worn (given timestamps for when it was worn)
	a. In progress

4. Create a dataframe that lists the names of the people who wore the mask for the required amount of time (or more) and another dataframe listing the people (or MaskID) that did not wear the mask for the required amount of time. 
	a. Using a threshold value for how long the mask should be on, we created this program around a sample community of students, who were expected to wear their mask for 6 hours (a week). **This code is located toward the beginning of the file.**

** NOTE: All realistically simulated data for humidity and temperature, as well as the calculation of hours and assignment of thresholds were done using research from a study conducted <https://www.ncbi.nlm.nih.gov/pmc/>**
