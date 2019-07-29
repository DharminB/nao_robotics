# nao_robotics
Software created for playing around with Nao robots

## Dependencies

### NAO python SDK
(Assuming Linux 64 bit is installed. 

1. **Download**

To install Nao python SDK, download `pynaoqi-python2.7-2.1.2.17-linux64` from [community website](https://community.ald.softbankrobotics.com/en/resources/software/former-nao-versions-python-naoqi-sdk).

2. **Extract**

Go to the directory where the downloaded file exists and extract 
```
tar -xvf pynaoqi-python2.7-2.1.2.17-linux64
```

Move the folder to `/opt` since that is a good practice
```
sudo mv pynaoqi-python2.7-2.1.2.17-linux64 /opt
```

3. **Install**

Extend environment variable called `PYTHONPATH` so that the computer can find 
this library.
```
export PYTHONPATH=${PYTHONPATH}:/opt/pynaoqi-python2.7-2.1.2.17-linux64 
```

This is a one time solution. In order to not do this everytime, this command can
be placed in `~/.bashrc`.

4. **Test**

Import `naoqi` in python command line. If no errors occur, installation was
successfull.
```
python2
import naoqi
```
