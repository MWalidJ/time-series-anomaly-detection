- link for the paper: https://iopscience.iop.org/article/10.1088/1741-2552/ab260c/pdf

Notes
* Maybe we dont need labels (unsupervised) since autoencoders learns features
	* Quote: "For example, autoencoders (AEs) learn a representation of the input data by trying to reproduce their input given some constraints, such as sparsity or the introduction of artificial noise"
* The paper suggests that raw data are sufficient and no need for preprocessing required.
	* Just to clarify: there is a difference between the use of preprocessing in the EEG setting and preprocessing in neural network terminologies. in neural networks its related  nerical stability and being model-friendly, like ( normalization, padding, encoding..etc) 
	* Thus, I suggest we start with raw data and see how it goes, and then we adjust based on the performance of the model
	* Quote: "According to our findings, the great majority of the reviewed papers preprocessed the EEG data before feeding it to the deep neural network or extracting features. Despite observing this trend, we also noticed that recent studies outperformed their respective baseline(s) using completely raw EEG data."
	* Quote: "While the answer depends on many factors such as the domain of application, we observed that in some cases raw EEG as input consistently outperformed baselines based using classically extracted features. For example, for seizure classification, recently proposed models using raw EEG data as input achieved better performances than classical baseline methods, such as SVMs with frequency-domain features. For this particular task, we believe following the current trend of using raw EEG data is the best way to start exploring a new approach."
* Depth of the network:
	* range between 4-10 layers
	* As we discussed, I suggest we start with small numbers and then adjust, based on performance 
* Although on CNNs, but they mostly fed the model with raw data, not features. 
* The following image contain
	* ![[Pasted image 20250420072115.png]]