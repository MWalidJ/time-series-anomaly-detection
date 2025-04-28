[Frontiers | Automatic Analysis of EEGs Using Big Data and Hybrid Deep Learning Architectures](https://www.frontiersin.org/journals/human-neuroscience/articles/10.3389/fnhum.2019.00076/full)


* This is a 3 pass architecture
	* 1st: Hidden Markov Model
	* 2nd: Deep Learning AutoEncoder
	* 3rd: Sequential Language Modeling
* mentions that there are **over 10 different electrode configurations and over 40 channel configurations** represented in the corpus, which poses a challenge for machine learning systems needing to adapt
	* For their initial study, they **focused on a subset of the data recorded using the Averaged Reference (AR) electrode configuration**44. This can be seen as a way to handle the variability in channel configurations by selecting a consistent subset.
	* **how can solve this issue? can we find a way to split the dataset into a way that categorize files based on number of channels?**
	* 