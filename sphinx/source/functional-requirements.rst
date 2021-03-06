2. Functional Requirements
==========================


2.1. Input
----------
 A valid submitted gene expression file has the following format :

 * Users have to submit three files.

 * For the file format, the file have to be json file.

 * The file should contain the condition of gene and gene expreession level value for each group condition. (e.g."R0001000014601":1.38128181929635). The condition names in both files must match. The details of the condition should be included in the information file.

2.2. Output
------------
2.2.1. Requirements Analyzing
******************************

 The web application displays a scatter plot when given gene expression files.
 
=== ============================================================================================== ======================================================================================================================== =========
NUM              RQ                                                                                                RA                                                                                                                    PRIORITY     
=== ============================================================================================== ======================================================================================================================== =========
1   The dots are sorted by color.The different tissue is indicated by different coloration         It is convenient for users to observe the correlation between the expression levels of two genes within the same tissue                                                   H
2   The details of the point where the mouse is located can be displayed                           Users can view the experimental conditions of the two genes                                                                                                                       H
3   Calculate the correlation coefficient of each tissue                                           Users can more intuitively determine the correlation between two gene expression levels                                       H
4   If the user submits an invalid file, the program will return an error message                  This reminds the user that the uploaded file is invalid                                                                      M
=== ============================================================================================== ======================================================================================================================== =========


2.2.2. Plot Analyzing
**********************
If the expression level of G2 increases with the increase of the expression level of G1, it means that G1 promotes the expression of G2; if it decreases, it inhibits the expression of G2.If the distribution of points of the same color is dense and the correlation coefficient is high, it means that the two genes are highly correlated; if the distribution of points of the same color is scattered, it means that their correlation is low.

 Our scatter plot model is as follows :

 .. image:: https://raw.githubusercontent.com/jerilmm/gene-expression/master/sphinx/source/img.png
