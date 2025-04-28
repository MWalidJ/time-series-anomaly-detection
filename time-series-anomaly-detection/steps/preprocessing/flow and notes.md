
here is the space to throw our ideas about the preprocessing steps needed:

first lets assume we 
1- loaded the raw data using mne
* raw = mne.io.read_raw_edf(filepath, preload=True)
2- preprocessing
* filtering start and end frequency (optional): 1-40 hz for example
* resampling: because the files might have different sampling rates (Hz)
	* this is needed for proper temporal learning and to use fixed-size windows
	* (This is assuring same number of samples per secon for all inputs)
	* It could be downsampling for computational efficiency purposes
	* Code:
			* raw.resample(256) # if we want to make the sampling to 256 
* Normalization
	* we do that because every patient have different signal strength
		* normalization assures same scale across all signals
		* in this way the model focuses on shape not size
	* Method
		* Z-score normalization
			* mean = 0 
			* std = 1 
	* Code
		* data = (data - data.mean(axis=1, keepdims=True)) / (data.std(axis=1, keepdims=True) + 1e-8)
* 