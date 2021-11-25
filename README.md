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

### Fpgrowth Steps

1.The first step is to search the database for instances of the itemsets. This step is identical to Apriori's first step. Support count or frequency of 1-itemset refers to the number of 1-itemsets in the database.

2.The FP tree is built in the second stage. To do so, start by making the tree's root. Null is used to represent the root.

3.Scanning the database and examining the transactions is the next stage. Examine the first transaction to determine the itemset included therein. The highest-counting itemset is at the top, followed by the next-lowest-counting itemset, and so on. It signifies that the tree's branch is made up of transaction itemsets arranged in descending order of count.

4.The database's next transaction is reviewed. The itemsets are sorted by count in ascending order. This transaction branch would share a common prefix to the root if any itemset of this transaction is already present in another branch (for example, in the first transaction).

This means that in this transaction, the common itemset is linked to the new node of another itemset.

5.The count of the itemset is also incremented as transactions occur. As nodes are formed and linked according to transactions, the count of both the common node and new node increases by one.

6.The next step is to mine the FP Tree that has been generated. The lowest node, as well as the links between the lowest nodes, are evaluated first. The frequency pattern length 1 is represented by the lowest node. From there, follow the FP Tree's course.
