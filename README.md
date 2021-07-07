# Predicting CPU usage with two different approaches

Here you can find how I've dealt with the task of predicting CPU usage with data from [this dataset](www.openml.org/d/197).

This data consists of 21 metrics describing from different angles the low-level tasks performed by a bunch of computers at some university department. The task is to predict the CPU usage, as a percentage. It is therefore a regression task.

I propose two different ways of dealing with the data. First one is to reduce the data's dimensionality through PCA. This data lends itself quite well to this path, as the three first principal components already gather 99% of the variability. Then, a simple regression is performed. The second approach I've taken is to first separate observations between those corresponding to an active CPU and to an inactive CPU. This implies combining a classifier and a regresor. This way I manage to scrap a 2% more in accuracy up`to 98%.
