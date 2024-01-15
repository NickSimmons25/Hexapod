# Hexapod
The following repo contains the software package required to simulate and control the Off-Kilter Solutions Hexapod. 

## Operating System
The code contained within this repository runs on WSL 2, Ubuntu 22.04.
This ensures that we have compatability with gazebo (assuming we want to use it). 
I also think an Ubuntu codebase allows us to utilise CUDA more easily - however, I could be wrong on this. 
These pieces of software require windows 11.
WSL and Ubuntu 22.04 install: https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-11-with-gui-support#1-overview
Linking WSL and windows vscode: https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-vscode
Remove other installed Ubuntu distros: https://askubuntu.com/questions/1261664/how-to-uninstall-the-wsl-installation-of-ubuntu-20-04-from-windows-10

## Installation Instructions
Repo setup instructions (assuming vscode):
1. Clone the git repository into your local files.
2. Ensure python is installed. By default, python 3.10.12 should come installed with Ubuntu 22.04.
```python3 -v```
3. Open the cloned repository in vscode, using the instructions provided in https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-vscode.
4. Create and activate a vscode virtual environment: https://code.visualstudio.com/docs/python/python-tutorial#:~:text=Create%20a%20virtual%20environment,-A%20best%20practice&text=Open%20the%20Command%20Palette%20(Ctrl,For%20this%20example%2C%20select%20Venv..
5. Install all required dependencies with the following command:
```pip install -r requirements.txt```
6. run main.py. If 'Hello, world!' is printed to console, the software is installed successfully!