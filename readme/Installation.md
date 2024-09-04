
## Install Python on Apple, Ubuntu and Window

### Apple : 
__Installation of Homebrew :__
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
__Installation of Python :__
```bash
brew install python
```
__Start a virtual environment:__
```bash
python3 -m venv myenv
source myenv/bin/activate
```
### Ubuntu (not manual)
__Check if Python is not already installed:__
```bash
python3 --version
```
__Update Ubuntu packets :__
```bash
sudo apt update
```
__Install Python :__
```bash
sudo apt install python3
```
__Start a virtual environment:__
```bash
sudo apt install python3-venv
python3 -m venv myenv
source myenv/bin/activate
```
### Ubuntu (manual)
__To install the Python package manager :__
```bash
sudo apt install build-essential libssl-dev libffi-dev python3-dev
```
__Download and extract the sources (Replace X Y Z with the desired version of Python :__
```bash
get https://www.python.org/ftp/python/X.Y.Z/Python-X.Y.Z.tgz
tar -xf Python-X.Y.Z.tgz
cd Python-X.Y.Z
```
__Configure and install :__
```bash
./configure --enable-optimizations
make
sudo make altinstall
```
### Window
__Install python on Window :__
```bash
[python.org](https://www.python.org/downloads/)
During the installation, check the box 'Add Python to PATH' so that Python is accessible via the command line.
Follow the instructions to complete the installation.
```
__Start a virtual environment:__
```bash
python -m venv myenv
myenv\Scripts\activate
```
[Intall Flask For the Project](./flask.md)