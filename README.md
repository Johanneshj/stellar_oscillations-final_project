**GITHUB repo for final project of course Stellar Oscillations: Techniques and Theory**

Step-by-step guide:

**Step 1:** Git clone this repo into a local folder. Copy the following into your terminal command line and hit enter "git clone https://github.com/Johanneshj/stellar_oscillations-final_project.git"

**Step 2:** Enter the folder and create a Python virtual environment (version 3.12.0 should work). I am using pyenv so for me to command is "pyenv virtualenv 3.12.0 venv-final_project. This will create a Python virtual environment version 3.12.0 with then name venv-final_project.

**Step 3:** Source your virtual environment: With pyenv, while being in the project folder, you can simply write "pyenv local venv-final_project". Otherwise you locate your folder and type "source venv-final_project/bin/activate".

**Step 4:** Enter the PBjam-teaching folder and run "pip install -r requirements.txt" in your command line. This will install all required Python packages in our venv.

**Step 5:** Open the pbjam.ipynb notebook and follow it cell-by-cell. 

**Step 6:** Enter the BASTA folder and type the following commands "mkdir -p ~/BASTA/grids" and "mkdir -p ~/BASTA/dust". 

**Step 7:** We will now download our grid of models: This is neatly done with the following command "BASTAdownload --gridpath grids --no-dustmaps validation"
