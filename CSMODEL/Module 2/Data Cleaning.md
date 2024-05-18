#csmodel


Raw data is inherently dirty. In data cleaning, incosistensies are fixed

Multiple representations
	different rpresentations of text may occur int he dataset
	use the unique() function to ensure that categorical vairables are correctrly represneted
	https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.drop_duplicates.html

incorrect datatype
	numberiocal values in the datatset may be represent as text or string
	use the info() function to check the datatype of each column 
	convert all variabels to their appropriate using apply() function to approparite column and use lambda function to convert each element to type
	astype() from numpy to typecast and apply to entire array

edfault values
	use default value for when data is missing or not applicable
	in pandas, missing values are represented as NaN or None
	![[Pasted image 20240514165112.png]]

Inconsistent format
	date and time may be recorded in inconsistent formats
		human error
		inconsistencies in data ollection and encoding

store results in a different variable
only if sure will you override the original one 
safest format is unix time to standardize date time values
	
data preprocessing
	
	![[Pasted image 20240514170930.png]]

Queryiung 
	use query function of pandas to write complex conditions for slecting appropriate info from dataset
	query() function queries the columns of a dataframe with a boolean expression
	alternative for using the bracker operator discussed during data representation
	query also can refer to row index
	![[Pasted image 20240514172030.png]]
![[Pasted image 20240514173016.png]]
![[Pasted image 20240514173617.png]]
![[Pasted image 20240514174528.png]]


### Continuation - 5/17

dropping entire rows columns through a threshold
	using a threshold value is dropping those return TRUE on the conditional that this certain element is < t where t is the threshold value
imputation 
	use median or average of other values as estimate of missing values
		ex: age of one person is missing, then use median age of all other people in the dataset to estimate the age o that person - missing age is likely the same as most commmon age in the dataset
		note tho to check dataset if good idea or not 
	inb categorical imputation, use mode as estimate for missing values
		not best paprice if no dominant value
		and values are approximately distribpute

binning
binning refers to a trechnique where data is grouped togfether into a series of categors
numerical data and binning catgericak data


outlier detection
extreme values in the dataset
these might be detected using diff approaches
	visualizsation techniques
	standard devatiu / z score
	precentiles
ex: 
	detect outliers plotting data points in a graph
	get the middle x percent of the data in a bell curve. anything outside the middle x percent is an outlier
	algorithm used in finding outliers graphically - not really discussed and out of course - but machine learning algorithm and is called random sample consensus. typically used for outlier detection 
	std dev - mean is center point of everything, std dev represents how far the sample is from the mean on average
	in standard deviaiton, if malayo from the mean of the bell curve. if your sample is more than 3 standard deviations away from the mean, then it is considered an outlier
	z test is one of the hypothesis test and lets you calculate the z score which is another way to pinpoint where the sample is. z score is usually 2 standadard fdevidations away
once detected outliuers
two approaches:
	1. drop them before doing analyusis. renive riws wutg iytkuers ti exclude them but good to keep them just not in the calculations
	2. use a cap - instead of dropping samples, we just cap / clamp within the desiered range. something like a cap on 3 starndard deviations away from the mean of the sample
consider tho: 
	mean is very robust for outliers
	this happens there is alarge amount of sample and like one of them is just an outlier. 
	there are many causes of outliers, byu removing or disregarding them , some important insights might be reomved from data
	common approach is calculate the median. median is less robust against outliers and more resistant. so use median 

One Hot Encoding
	some data modelling tehcniques include machine learning algos wihch require different data rperesentaiton. 
	boolean representation where each propert is represented as a column where the value is 1 if it is tgrue and 0 otherwise
	content based recommender systems the item rofile was represented as a boolean vector
think of it like binary:
Item  | Color 
1 | Red
2 | Blue

in one hot is:
Red | Green | Blue
1 | 0 | 0
0 | 0 | 1 

Reconmmender systems - recommends that something an object is something a user would use based on past data. 

used for computer network architectures. 


Log Transformation
	 make non normal data to more normally distributed
	 most data we'll find is normally distrvured, soenm uniform, some poisson,
		non normal is starts high, starts shringking or starts low, starts rising. these are exponential
	most data analysis techqnieues need the use of normal distrivbution 


Aggreggation 
	sum or mean might be extravted from numberical data
	mode within a group can be used for categorical data

Column Transmfonation
	transform columns to extract better information from the dataset
	so like how a full name can be separated to a first name and last name 

Feature sacling 
	differnt variables may have different ranges
	some algos will be afected if one varibale overpowers others (e.g., scatter plot)'
	ex: euclidean distance will be affecetd f the scale of the vairbales are not equal 
	normalzaition scales all feautres into a range of 0 to 1.
		(x - x_min) / (x_max - x_min)
	Note that this is susceptible to outliers
	standardiaztion z score measures distance of each poitn from the mean :
		(x- mew )/ sigma
	note: less sucpetible to outliers since it considertds stardarnd vdivneation
	














































































