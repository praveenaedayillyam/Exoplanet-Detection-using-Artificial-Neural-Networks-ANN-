# Exoplanet-Detection-using-Artificial-Neural-Networks-ANN-

 ### Problem Statement
- NASA’s Kepler Space Telescope collected light curve data to detect exoplanets (planets outside our solar system). Traditionally, identifying candidate exoplanets required manual inspection, which is slow and error-prone.
- The challenge: automatically classify candidate signals as real exoplanets or false positives using AI/ML.
- Dataset Source: NASA Exoplanet Archive / Kepler Mission Data (Caltech/IPAC).

- Type: Tabular data with astrophysical and observational features.

- 	Important columns:

- ○	koi_disposition → Target label (Confirmed Planet, False Positive, Candidate).

- ○	Orbital parameters: koi_period, koi_duration, koi_depth

- ○	Planetary radius: koi_prad

- ○	Stellar properties: koi_steff (temperature), koi_slogg (gravity), koi_srad (radius)

- ○	Transit signal quality: koi_model_snr

### Methodology<br>
1.	Data Cleaning & Preprocessing<br>

- ○	Removed rows with NaN values.

- ○	Selected relevant numerical features.

- ○	Encoded target labels into binary/multiclass format.

- ○	Normalized feature values for neural network training.<br>

2.	Model Architecture (ANN)<br>

- ○	Input layer: all selected features.

- ○	Hidden layers: Dense layers with ReLU activation.

- ○	Output layer: Sigmoid Activation<br>

3.	Training & Validation<br>

- ○	Dataset split using train_test_split.

- ○	Loss function: Cross-entropy.

- ○	Optimizer: Adam.

- ○	Metrics tracked: Precision, Recall, Accuracy.<br>

4. Evaluation<br>
	
- ○	Precision : 0.980017364025116
- ○	Recall : 0.9082125425338745
- ○	Accuracy : 0.9414780139923096

### Results
- 	The ANN successfully learned patterns in orbital, stellar, and transit features to identify exoplanets.

- 	Achieved strong performance in accuracy, precision, and recall, showing reliability in automatic classification.

- Impact
- 	Automates exoplanet detection from NASA mission data.

-  Reduces manual effort and speeds up discovery.

- 	Scales well to large datasets like Kepler and TESS, where millions of light curves exist.

- 	Demonstrates the power of AI in astrophysics and space exploration.

- ### In this Folder
-  notebook.ipynb :   work & experiments - Code

- 	dataset.zip : input data

- 	model.h5 : final trained model
