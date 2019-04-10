2. Functional Requirements
==========================


2.1. Input
----------
 A valid submitted gene expression file has the following format :

 * Users have to submit three json files.

 * For the file format, the file have to be json file.

 * The file should contain the condition of gene and gene expreession level value for each group condition. (e.g."R0001000014601":1.38128181929635). The condition names in both files must match. The details of the condition should be included in the information file.

2.2. Output
------------

 The web application displays a scatter plot when given a gene expression file.
=== ===================================================================== ================================================================================= =======
num              RQ                                                                 RA                                                                                                                    PRIORITY     
=== ===================================================================== ================================================================================= =======
1      Generate a scatter plot showing the correlation of gene expression The X-axis is the expression level of G1 and Y-axis is the expression level of G2  H
2      李四     未填写
=== ===================================================================== ================================================================================= =======

 The scatter plots displays gene correlations.The X-axis is the expression level of G1 and Y-axis is the expression level of  G2.We use different colors to represent different experiments under different conditions.If the expression level of G2 increases with the increase of the expression level of G1, it means that G1 promotes the expression of G2; if it decreases, it inhibits the expression of G2.If the distribution of points of the same color is dense and the correlation coefficient is high, it means that the two genes are highly correlated; if the distribution of points of the same color is scattered, it means that their correlation is low.When our mouse touches some of these dots, we can get the  related information of the dot.

 Our scatter plot model is as follows :

 .. image:: https://raw.githubusercontent.com/jerilmm/gene-expression/master/sphinx/source/img.png
