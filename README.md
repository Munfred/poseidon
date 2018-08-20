# poseidon pumps and microscope


## To run it on raspbian

To run `gui.py` in a raspberry pi with a fresh install of raspian a few packaged need to be installed first

```
sudo apt-get install python3-pyqt5

# now need to use python3.5 gui.py to invoke the python3 that has pyqt5!

pip3 install --upgrade -pip
pip3 install pyserial
pip3 install opencv-python

# opencv requires a some extra binaries 

sudo apt-get install libatlas-base-dev
sudo apt-get install libjasper-dev
sudo apt-get install libqtgui4
sudo apt-get install libqt4-qt3support
sudo apt-get install libqt4-test

python3.5 gui.py
```


## Installing pyinstaller on windows to compile binaries

To use pyinstaller on windows it's better to use it with python 3.4 
because there are unsolved dependency errors in later versions 
Binary for python 3.4.2 (later versions don't have binaries): https://www.python.org/downloads/release/python-342/


Then to install PyQt5 python 3.4 on windows you need to install it from the installer, 
not form pip, as described here:
https://stackoverflow.com/questions/22640640/how-to-install-pyqt4-on-windows-using-pip
http://pyqt.sourceforge.net/Docs/PyQt5/installation.html
https://sourceforge.net/projects/pyqt/

Then the rest of the dependencies install without problems
```
python -m pip install pyserial
python -m pip install opencv-python
```

To run: `python gui.py`
