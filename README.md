# Apropri-fpgrowth

The Apriori Algorithm is commonly used for frequent pattern mining, and FP-growth is an upgraded version of it (AKA Association Rule Mining). It's an analytical technique for identifying common patterns or correlations in data sets.

Han proposed the FP-Growth Algorithm, which is an efficient and scalable method for mining the entire set of frequent patterns by pattern fragment growth, which uses an extended prefix-tree structure for storing compressed and crucial information about frequent patterns called the frequent-pattern tree.

### Steps for Apriopri
1.Calculating the amount of support for each item separately.

2.Choosing a support threshold.

3.Choosing the most frequently used things.

4.Obtaining the assistance of the frequently occurring itemsets.

5.Rep with larger sets.

6.Calculate confidence using Association Rules.

7.Calculate the lift.

### Shortcomins of Apriopri Algorithms
1.Apriori requires the creation of candidate itemsets. If the database's itemset is vast, these itemsets may be numerous.
2.Multiple scans of the database are required by Apriori to check the support of each itemset generated, which results in significant expenses.
