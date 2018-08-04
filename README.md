# poseidon pumps and microscope

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
