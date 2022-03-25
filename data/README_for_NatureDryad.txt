README.txt for the manuscript
"Mutation predicts 40 million years of fly wing evolution"
provsionally accepted at Nature, June 27, 2017.

This archive consists of three files: 
eigenvectorsNature.csv  	This has the eigenvectors used to score each data set.
speciesNature.csv		This file has the x,y coordinates for the 12 landmarks in the species data set. 
AllAlignedNature.csv		This file has the scores for the aligned landmark data on the first 20 principal component vectors in EigenvectorsNature.csv for the species, mutation and Wabassso data sets. 

  **************************************
The variables in eigenvectorsNature.csv are:
_TYPE_		type of Variates on this line
_NAME_		name of variable of vector
lmlax,lmlay 1-12	Names of x and y coordinates of the 12 landmark point on each wings. 

When _TYPE_=COV, this is the covariance matrix subjected to principal components analysis
When _TYPE_=EIGENVAL entries are the first 21 eigenvalues of the covariance matrix
When _TYPE_=SCORE, record is the eigenvector corresponding to the _name_ principal component. 

  ***************************************

The variables in speciesNature.csv are:
flyunique	String with name of the image file from which the data were extracted.  Original files are available from David Houle (dhoule@bio.fsu.edu).
lncs		natural log of centroid size in mm, times 100.
cslmmm		centroid size of the specimen in mm.
lmlax,lmlay	x and y coordinates of the 12 landmark point on each of the species wings.  
Species		code for identity of the species
tiff		name of the original image (TIFF) file
CPfile		name of the file that holds the spline curves fit to the wing
Perp		Name of person who imaged the wing
Date		date the wing image recorded
Time		time the wing image recorded
Tags		Additional information about the stock or source of the fly imaged
Sex		Sex of fly
pixelsize	centroid size in the number of pixels in the original image

  ***************************************

The variables in AllAlignedNature.csv 
flyunique	String to enable us to locate the original image the data is derived from.
group		Code for data set. D= species data set. Gw=G matrix data set (Wabasso Florida). M=mutation data set.
cslmmm		centroid size of the specimen in mm.
Prin1 - Prin20	Scores on the first 20 eigenvectors in the file eigenvectorsNature.csv, times 1000.
lncs		natural log of centroid size in mm, times 100.

Original data on speciemens in the Gw and M data sets is posted at Dryad (doi:10.5061/dryad.3b7g5, doi: 10.5061/dryad.hb37q)
