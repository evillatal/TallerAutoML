# TallerAutoML
Taller Introductorio de Machine Learning y AutoML

Para el desarrollo del taller es necesario instalar ciertas librerias. A continuacion se detalla los pasos del software a instalar para Windows y Linux

# WINDOWS 10
1) Open PowerShell as Administrator and run: 
	Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
2) Restart Windows
3) Open Windows Store
4) Install Ubuntu 18.04 LTS
5) Initialize Ubuntu
6) Create user and password
7) Update & upgrade distro's packages
	>> sudo apt update && sudo apt upgrade
8) Install the most recent version of Python3-Pip and python3-dev
	>> sudo apt install python3 python3-pip python3-dev
9) Now, we create a Python virtual environment to manage our projects
   
   - first we need access to the virtualenv command which we can install with pip. 
	>> sudo -H pip3 install --upgrade pip
	>> sudo -H pip3 install virtualenv
	(The -H flag ensures that the security policy sets the home environment variable to the home directory of the target user)
	
   - With virtualenv installed, we can start forming our environment. Create and move into a directory where we can keep our project files.
   >>  mkdir ~/python_projects
   >> cd python_projects
   
   - Within the project directory, we’ll create a Python virtual environment
   >> virtualenv project_env
   (This will create a directory called project_env within your python_projects directory)
   
   - we need to activate the virtual environment
   >> source project_env/bin/activate
   (now we are ready to install Jupyter into this virtual environment)
   
10) Install Jupyter within the activate environment
	>> pip install jupyter
	( use pip instead of pip3, even if we are using Python 3. The virtual environment’s copy of the tool is always named pip, regardless of the Python version)
	
11) Install all dependencies of auto-sklearn manually with:
	>> sudo apt-get install build-essential swig
	>> sudo apt-get install curl   (If not installed jet)
	>> curl https://raw.githubusercontent.com/automl/auto-sklearn/master/requirements.txt | xargs -n 1 -L 1 pip install
	>> pip install matplotlib
	
12) Install Auto-sklearn
	>> pip install auto-sklearn
	
13) Para copiar un archivo del sistema de windows al sistema de archivos de Linux:
	>> cp /mnt/c/[source path and filename]  [destination path and filename] 
	

# Linux

1) Update & upgrade distro's packages
	>> sudo apt update && sudo apt upgrade
2) Install the most recent version of Python3-Pip and python3-dev
	>> sudo apt install python3 python3-pip python3-dev
3) Now, we create a Python virtual environment to manage our projects
   
   - first we need access to the virtualenv command which we can install with pip. 
	>> sudo -H pip3 install --upgrade pip
	>> sudo -H pip3 install virtualenv
	(The -H flag ensures that the security policy sets the home environment variable to the home directory of the target user)
	
   - With virtualenv installed, we can start forming our environment. Create and move into a directory where we can keep our project files.
   >>  mkdir ~/python_projects
   >> cd python_projects
   
   - Within the project directory, we’ll create a Python virtual environment
   >> virtualenv project_env
   (This will create a directory called project_env within your python_projects directory)
   
   - we need to activate the virtual environment
   >> source project_env/bin/activate
   (now we are ready to install Jupyter into this virtual environment)
   
4) Install Jupyter within the activate environment
	>> pip install jupyter
	( use pip instead of pip3, even if we are using Python 3. The virtual environment’s copy of the tool is always named pip, regardless of the Python version)
	
5) Install all dependencies of auto-sklearn manually with:
	>> sudo apt-get install build-essential swig
	>> sudo apt-get install curl   (If not installed jet)
	>> curl https://raw.githubusercontent.com/automl/auto-sklearn/master/requirements.txt | xargs -n 1 -L 1 pip install
	>> pip install matplotlib
	
6) Install Auto-sklearn
	>> pip install auto-sklearn


