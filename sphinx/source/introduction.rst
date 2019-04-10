
1. Introduction
===============



 We have to build a web application which can generate a gene expression scatter plot given relevant JSON files as input.  This document is intent to specify a set of requirements for our project.


1.1. Purpose
--------------
 Generate a scatter plot based on two gene expression level samples to observe the expression level of two genes in the different experimental condition. It can help biologists to analyze experimental data.


1.2. Overview
--------------
 The remainder of the document is organized as follows：first,we introduce the overall descirption.Then we analyze the product requirements。Finally, we analyzed the constraints and some change cases of the software.

1.3. Overall Description
-------------------------
1.3.1. User Characteristics
****************************
 * clients: Biologists who are using web application to processing experimental data. 

 * web maintainers: Computer technicians skilled in python and github.

1.3.2. Product Features
************************
  The web application has a simple homepage with two buttons [Upload] and [Reset]. Our scientists upload two sample files of the expression levels of two genes G1 and G2 and the details of their conditions. Accepting these files, the software will return a scatter plot of gene expression correlation whose X-axis is G1 and Y-axis is G2. If an invalid file is given, the web application returns a page informing the user to provide the correct format.

1.4. Terminologies
-------------------
 In order to introduce the project and specify the requirements in detail, this section will explain some terminologies so that the clients and maintainers have better understanding of the content of the project.
 
  *JavaScript Object Notation(json)* - A lightweight data interchange format based on the JavaScript language.
  
  *Invalid file* - The document type is not json and the contents of the files can not represent the level of gene expression.

