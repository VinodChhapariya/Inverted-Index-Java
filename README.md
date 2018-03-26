# Inverted-Index-Java
# CONTENTS OF THIS FILE
 * Introduction
 * Requirements
 * Steps To Execute The Code
 * Troubleshooting

# INTRODUCTION

Problem Description: "https://moodle.iith.ac.in/mod/assign/view.php?id=1268"

# SYSTEM REQUIREMENTS

-JRE1.8 and above
-Eclipse IDE 

-ExternalJar File
 * org.tartarus.snowball.jar 
 * jcommon-0.8.0.jar
 * jfreechart-1.0.6.jar
 
# STEPS TO EXECUTE THE CODE :

-Crawled files from first assignment are to be placed in directory named "Iutput" in project folder. 

-Stop Words file is required by name "StopWords.txt" to create index I2.

# Section I

-Inverted indices I1 to I4(Inverted_Index_1.txt,Inverted_Index_2.txt,Inverted_Index_3.txt,Inverted_Index_4.txt) are created as text files as per the requirements and following parameters are calculated on each of the indices.  
	1) Number of Terms
 	2) Maximum Length of Postings List
	3) Minimum Length of Postings List
	4) Average Length of Postings List
	5) Size of the file that stores the index

# Section II

	-Three Text files(Most_Frequent_K_Words.txt,Median_K_Words.txt,Least_Frequent_K_Words.txt) generated for each of the below K words and comptutation is performed on all the four indices generated in Section I.  

	-Most Frequent K (K=20) words, size of posting list of each of these K words and average gap between the documents are computed. 

	-Median K (K=20) words, size of posting list of each of these K words and average gap between the documents are computed. 

	-Least Frequent K (K=20) words, size of posting list of each of these K words and average gap between the documents are computed. 

# Section III

-Graph for 1000 terms which have highest frequency in the collection is plotted (computation performed on Index-4). 
	
	X-axis -> log of the rank of the term in non-increasing collection frequency ordering.  
	
	Y-axis -> log of collection frequency of the term.

# Section IV

-Graph for number of tokens already found and vocabulary size is plotted (computation performed on Index-4). 
	
	X-axis -> log of the number of tokens already seen.  
	
	Y-axis -> log of the vocabulary size.

# TROUBLESHOOTING

Exceptions handled:

	-IOException - Exception occurs when reading or writing to file or console. 
	-FileNotFoundException- Exception occurs when file/directory path is wrong or file not exist in given path. 
	-StemmerException - Exception occurs when stemmer not able to recognize the token or any stemming related problem.
	-ArryaIndexOutOfBoundException - Exception occurs when Location beyod predefined size is accessed by ArrayList.
