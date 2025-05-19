**GITHUB repo for final project of course Stellar Oscillations: Techniques and Theory**

Step-by-step guide:

**Step 1:** Git clone this repo into a local folder. Copy the following into your terminal command line and hit enter "git clone https://github.com/Johanneshj/stellar_oscillations-final_project.git"

**Step 2:** Enter the folder and create a Python virtual environment (version 3.12.0 should work). I am using pyenv so for me to command is "pyenv virtualenv 3.12.0 venv-final_project. This will create a Python virtual environment version 3.12.0 with then name venv-final_project.

**Step 3:** Source your virtual environment: With pyenv, while being in the project folder, you can simply write "pyenv local venv-final_project". Otherwise you locate your folder and type "source venv-final_project/bin/activate".

**Step 4:** Enter the PBjam-teaching folder and run "pip install -r requirements.txt" in your command line. This will install all required Python packages in our venv.

**Step 5:** Open the pbjam.ipynb notebook and follow it cell-by-cell. 

**Step 6:** Enter the BASTA folder and type the following commands "mkdir -p ~/BASTA/grids" and "mkdir -p ~/BASTA/dust". 

**Step 7:** We will now download our grid of models: This is neatly done with the following command "BASTAdownload --gridpath grids --no-dustmaps validation". The grid is ~5 GB so this might take some time.

**Step 8:** Now we create our frequency xml file: Our list of frequencies generated in the notebook should be available in the data/freqs folder. Enter this folder and type "python3" into the terminal. This will open a python environment in the terminal. Here you then run "from basta import fileio; fileio.freqs_ascii_to_xml('.', 'KIC9635649')", *replace KIC9635649* with your ID. To exit the python environment type "exit()". You should now have a file name fx "KIC9635649.xml" in the freqs folder. This file we will rename to simply "9635649.xml" - that is just the ID.xml.

**Step 9:** Next we will create our BASTA input file with the python script create_inputfile.py". This file is tuned for my showcase star so you will need to do some tweaks yourself. Familiarize yourself with the script and use the BASTA documentation for more help. When ready hit and enter "python3 create_inputfile.py" in your terminal.
