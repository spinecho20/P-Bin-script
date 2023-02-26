#README 
This file describes the computer software implementation of Peak Bin(P-Bin), which is a combination of the classic peak-picking and binning procedures as described in the manuscript “Combination of Peak-picking and Binning for NMR Based Metabonomics Study ” (Chai et al. (2023)) 

#What is P-Bin
Binning or bucketing is a important precedure in NMR-based metabonomic analysis such as group classification or biomarker identification. Binning divides an NMR spectrum into many regions, and the integrations of these regions are sent to the following processing steps. P-Bin is a combination of the classic peak-picking and binning procedures. This method searches local maxima in each spectrum and uses them as the center of the bins. The digital range (size) of initial bins is suggested to be about half of the linewidth of a selected reference peak.The location of each peak defined by peak-picking is used as the center of the individual bin. The bin size and value are a few data points and integration of the corresponding intensities. P-Bin is expected to keep all spectral information associated with the peaks and significantly reduce the data size as the spectral regions without peaks are not considered. 

#INSTALLATION
P-Bin an be performed on any platform with Python (V3.9 or newer) that calls Python API in the Topspin(V4.1.4 or newer) environment.Python package and version required are listed as follow. You can also check requirment and download the package(bruker-nmr-api 1.1 & bruker-topspin-rest-api 1.0.0) on the Bruker websit (https://www.bruker.com/en/products-and-solutions/mr/nmr-software/topspin/topspin-python-interface.html) 
Package                 Version 
----------------------- --------- 
bruker-nmr-api          1.1 
bruker-topspin-rest-api 1.0.0 
certifi                 2021.10.8 
cycler                  0.11.0 
fonttools               4.31.2 
kiwisolver              1.4.2 
matplotlib              3.5.1 
numpy                   1.22.3 
packaging               21.3 
Pillow                  9.0.1 
pyparsing               3.0.7 
python-dateutil         2.8.2 
six                     1.16.0 
urllib3                 1.26.9 

extra package for P-Bin
openpyxl				3.0.9
tk						8.6.11



#Documentation
##Spectra preprocessing 
	phease 
	baseline correction 
	calibration 
	peak picking 

##Path file   
	Fill parameter in the ExamplePath file (xlsx) that cantain the permenents of Bin Size,Search Window (ppm),Peak occurrence threshold and Spectra Paths

##Run script 
	import the ExamplePath file
 	The intgral results would stored in Example Paths_P-Bin.xlsx

#Citing P-Bin
If you find P-Bin useful in your research please cite the package as:


#Getting Help
You can ask question on and request help feel free to email the creator of P-Bin directly.