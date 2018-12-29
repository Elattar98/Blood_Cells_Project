## Project Overview

Welcome to my capstone project in the ML Nanodegree! The goal of this project is to make classifier capable of taking an image of white blood cells and predict its respective type.  


## Project Instructions

### Instructions

1. (Optional) Download the original Blood Cells dataset.
```	

2. Download the data after take a subset of the training data to be used as validation data. If you are using a Windows machine, you are encouraged to use 7zip to extract the folder.

3. (Optional) If you plan to install TensorFlow with GPU support on your local machine, follow the guide to install the necessary NVIDIA software on your system. If you are using an EC2 GPU instance, you can skip this step.

4. Optional) If you are running the project on your local machine (and not using AWS), create (and activate) a new environment.

5. (Optional) __If you plan to install TensorFlow with GPU support on your local machine__, follow [the guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.  If you are using an EC2 GPU instance, you can skip this step.

6. (Optional) **If you are running the project on your local machine (and not using AWS)**, create (and activate) a new environment.

	- __Linux__ (to install with __GPU support__, change `requirements/cells-linux.yml` to `requirements/cells-linux-gpu.yml`): 
	```
	conda env create -f requirements/cells-linux.yml
	source activate cells-project
	```  
	- __Mac__ (to install with __GPU support__, change `requirements/cells-mac.yml` to `requirements/cells-mac-gpu.yml`): 
	```
	conda env create -f requirements/cells-mac.yml
	source activate cells-project
	```  
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/cells-windows.yml` to `requirements/cells-windows-gpu.yml`):  
	```
	conda env create -f requirements/cells-windows.yml
	activate cells-project
	```

7. (Optional) **If you are running the project on your local machine (and not using AWS)** and Step 6 throws errors, try this __alternative__ step to create your environment.

	- __Linux__ or __Mac__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`): 
	```
	conda create --name cells-project python=3.5
	source activate cells-project
	pip install -r requirements/requirements.txt
	```
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`):  
	```
	conda create --name cells-project python=3.5
	activate cells-project
	pip install -r requirements/requirements.txt
	```
	
8. (Optional) **If you are using AWS**, install Tensorflow.
```
sudo python3 -m pip install -r requirements/requirements-gpu.txt
```
	
9. Switch [Keras backend](https://keras.io/backend/) to TensorFlow.
	- __Linux__ or __Mac__: 
		```
		KERAS_BACKEND=tensorflow python -c "from keras import backend"
		```
	- __Windows__: 
		```
		set KERAS_BACKEND=tensorflow
		python -c "from keras import backend"
		```

10. (Optional) **If you are running the project on your local machine (and not using AWS)**, create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `cells-project` environment. 
```
python -m ipykernel install --user --name cells-project --display-name "cells-project"
```

11. Open the notebook.
```
jupyter notebook Blood_Cells.ipynb
```

12. (Optional) **If you are running the project on your local machine (and not using AWS)**, before running code, change the kernel to match the cells-project environment by using the drop-down menu (**Kernel > Change kernel > cells-project**). Then, follow the instructions in the notebook.

__NOTE:__ While some code has already been implemented to get you started, you will need to implement additional functionality to successfully answer all of the questions included in the notebook. __Unless requested, do not modify code that has already been included.__


