Setup AGX Orin:

1, Install Jetpack 6 using NVIDIA's SDK Manager, from an X86 Ubuntu 20.04 via USB (hold Recovery and Reset for 2 seconds)

2, Change Power mode to MAXN

3, Install Chromeium via Ubuntu Software app

4, Install jtop: `sudo apt install python3-pip`, `sudo pip3 install jetson-stats`

5, Install OpenCV with Cuda: `chmod +x install_OpenCV_4.10.0_with_cuda_on_Jetpack_6.sh`, `sudo ./install_OpenCV_4.10.0_with_cuda_on_Jetpack_6.sh`

6, Install warp: `https://www.warp.dev/download`

7, Install VS Code: `https://code.visualstudio.com/download`

8, Install curl: `sudo apt install curl`

9, Install Mojo/Max: `curl -s https://get.modular.com | sh -`, `python3 -m venv max-venv && source max-venv/bin/activate`, `modular auth`, `modular install max`, `MAX_PATH=$(modular config max.path) \
  && python3 -m pip install --find-links $MAX_PATH/wheels max-engine`, `MAX_PATH=$(modular config max.path) \
  && BASHRC=$( [ -f "$HOME/.bash_profile" ] && echo "$HOME/.bash_profile" || echo "$HOME/.bashrc" ) \
  && echo 'export MODULAR_HOME="'$HOME'/.modular"' >> "$BASHRC" \
  && echo 'export PATH="'$MAX_PATH'/bin:$PATH"' >> "$BASHRC" \
  && source "$BASHRC"`

*Do not use U.S. apt mirror
