# econ3916-lab19-random-forests
# Tree-Based Models: Random Forests
# Objective
I compared how well tree-based and linear models predict house values in the California Housing dataset.
# Methodology
- I trained a single decision tree, OLS, Ridge, and a random forest on the same training data and evaluated them on the same test set.
- I compared the forest’s impurity-based feature importance (MDI) with permutation importance on the test set.
- I used cross-validation to tune the maximum tree depth and the number of features considered at each split.
- I used two rounds of AI prompts to build a feature-importance chart and checked the function’s results against my calculations for the forest and a separate decision tree.
# Key findings
- I got a test R² of 0.6161 for the single tree, 0.5758 for Ridge, and 0.8044 for the random forest. After tuning, the forest’s test R² rose to 0.8116.
- Latitude had an MDI score of 0.0889. Shuffling Latitude lowered the forest’s test R² by 0.4465 on average. Latitude ranked higher by permutation importance than by MDI.
- The final chart function returned the same features, in the same order and with the same importance values, as my checks for both models.
