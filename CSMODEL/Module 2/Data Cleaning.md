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
