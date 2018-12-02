## Project Overview

Welcome to my capstone project in the ML Nanodegree! The goal of this project is to make classifier capable of taking an image of Fruit and predict its respective category. 
## Project Instructions

### Instructions

1. (Optional) Download the original [fruit dataset](https://github.com/Horea94/Fruit-Images-Dataset). 

2. Download my version of the data after take a subset of the training  data  to be used as validation data. [my fruit dataset](https://github.com/mustafa150116/fruit_dataset).
Unzip the folders of mytrain1 ,mytrain2 and mytrain3 and place all 81 subfolders in the repo, at location `path/to/Capstone Project/fruits-project/data/fruit_images/mytrain`.
Unzip the folder of myvalid and place all 81 subfolders in the repo, at location `path/to/Capstone Project/fruits-project/data/fruit_images/myvalid`.
Unzip the folders of Test1 ,Test2 and place all 81 subfolders in the repo, at location `path/to/Capstone Project/fruits-project/data/fruit_images/test`.
If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

3. (Optional) __If you plan to install TensorFlow with GPU support on your local machine__, follow [the guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.  If you are using an EC2 GPU instance, you can skip this step.

4. (Optional) **If you are running the project on your local machine (and not using AWS)**, create (and activate) a new environment.

	- __Linux__ (to install with __GPU support__, change `requirements/fruit-linux.yml` to `requirements/fruit-linux-gpu.yml`): 
	```
	conda env create -f requirements/fruit-linux.yml
	source activate fruit-project
	```  
	- __Mac__ (to install with __GPU support__, change `requirements/fruit-mac.yml` to `requirements/fruit-mac-gpu.yml`): 
	```
	conda env create -f requirements/fruit-mac.yml
	source activate fruit-project
	```  
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/fruit-windows.yml` to `requirements/fruit-windows-gpu.yml`):  
	```
	conda env create -f requirements/fruit-windows.yml
	activate fruit-project
	```

7. (Optional) **If you are running the project on your local machine (and not using AWS)** and Step 6 throws errors, try this __alternative__ step to create your environment.

	- __Linux__ or __Mac__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`): 
	```
	conda create --name fruit-project python=3.5
	source activate fruit-project
	pip install -r requirements/requirements.txt
	```
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`):  
	```
	conda create --name fruit-project python=3.5
	activate fruit-project
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

10. (Optional) **If you are running the project on your local machine (and not using AWS)**, create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `fruit-project` environment. 
```
python -m ipykernel install --user --name fruit-project --display-name "fruit-project"
```

11. Open the notebook.
```
jupyter notebook fruit_app.ipynb
```

12. (Optional) **If you are running the project on your local machine (and not using AWS)**, before running code, change the kernel to match the fruit-project environment by using the drop-down menu (**Kernel > Change kernel > fruit-project**).