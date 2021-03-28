# Objective

Detect and locate tables inside a page using DNN, then parse the table to extract a dataframe that should not lose any information and structure of the table. The output should be an excel file containing the extracted table.


Assignment 3:

Instead of passing entire pdf book to parse for table, extracting single page from pdf and using that single page to parse the pdf has resulted in better extraction of tables.

**Total 152 tables were extracted with only few mistake table

Solution and explaination is present in assign_2.ipynb

Output is present in output_final.zip file

# Alternate Method used :
 
Using camelot library table data extraction was extremely bad for the PDF used.

According to research paper "DeCNT: Deep Deformable CNN for Table Detection", creating a system which is able to detect tables and its content in images will be more suited in extraction of table from PDF or any kind of file, since converting of file in image is easy and will result in better data collection.

Similar method is used in CascadeTabNet, which detect table in images using MMdetection framework in following steps:
1. Detectino of table boundary in image.
2. Table classification (border or borderless)
3. Structure detection of table and data.

-Trying to detect tables in steps is much better method than detecting and extracting in one step. Detection of data in step may cause mix match of data if multiple tables are present on the page or incomplete extractino of table. 
-Extracting tables in multiple steps also has advantage of dealing with tables of unconventional format.
