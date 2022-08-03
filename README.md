Install_OpenCV_RaspberryPi 

# Installing OpenCV on Raspberry Pi 

    sudo raspi-config 

That will open the Raspberry PI configuration tool window. Select Advanced Options and hit Enter.    
The new window that appears, select Expand Filesystem and hit Enter.
# Install OpenCV dependencies 

    sudo apt update
--------------------------------------------------------------------
    sudo apt upgrade
--------------------------------------------------------------------
    sudo apt install build-essential cmake pkg-config
----------------------------------------------------------------------
    sudo apt install libjpeg-dev libtiff5-dev libjasper-dev libpng-dev
------------------------------------------------------------------------
    sudo apt install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev
    sudo apt install libxvidcore-dev libx264-dev
--------------------------------------------------------------------------
    sudo apt install libfontconfig1-dev libcairo2-dev
    sudo apt install libgdk-pixbuf2.0-dev libpango1.0-dev
    sudo apt install libgtk2.0-dev libgtk-3-dev
    
--------------------------------------------------------------------------
    sudo apt install libatlas-base-dev gfortran
---------------------------------------------------------------------------
    sudo apt install libhdf5-dev libhdf5-serial-dev libhdf5-103
    sudo apt install libqt5gui5 libqt5webkit5 libqt5test5 python3-pyqt5
---------------------------------------------------------------------------
    sudo apt install python3-dev
---------------------------------------------------------------------------
    sudo apt-get install python3-pip
---------------------------------------------------------------------------
    sudo pip3 install virtualenv virtualenvwrapper
---------------------------------------------------------------------------
    nano ~/.bashrc
---------------------------------------------------------------------------
Add the following lines at the bottom of the file.

    # virtualenv and virtualenvwrapper
    export WORKON_HOME=$HOME/.virtualenvs
    export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
    source /usr/local/bin/virtualenvwrapper.sh
    
 -----------------------------------------------------------------------------
 Save the file (Ctrl + S, then Exit (Ctrl + X).
 
    source ~/.bashrc
-------------------------------------------------------------------------------
create a virtual environment for our projects.   
mkvirtualenv yourvirtualenv_name -p your python3 path
## example
    mkvirtualenv venv_atul -p python3
--------------------------------------------------------------------------------
Activate your virtualenv using cmd
source yourvenv_name/bin/activate
ex-   
    source /venv_atul/bin/activate
    
---------------------------------------------------------------------------------
Inside the virtual environment, you can now install OpenCV. Execute the command below.
    pip3 install opencv-python


Done 
    ### IOT DEVELOPER
    ### Atul kumar
