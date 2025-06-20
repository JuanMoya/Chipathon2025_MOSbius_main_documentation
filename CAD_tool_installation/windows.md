# Installation Steps for Windows

The Docker image used in this 2025 Chipathon is pre-packaged Docker container provided by Harald Pretl's lab **IIC-OSIC-TOOLS**: https://github.com/iic-jku/iic-osic-tools

First, a block diagram with the main installation steps:
<p align="center">
   <img src="./img/Installation_flow.png" width="600" />
</p>  

GUI-based tool setup:

1) Assuming that you have installed on your Windows machine **<ins>Windows Powershell</ins>**:

   a) Create a folder where you will pull Harald Pretl's Docker image.

   b) Clone Harald Pretl's Docker image from: https://github.com/iic-jku/iic-osic-tools with the following command:
  ```
  git clone https://github.com/iic-jku/IIC-OSIC-TOOLS.git
  ```
<p align="center">
   <img src="./img/cloned_repo.png" width="600" />
</p>  

2) Download Docker: https://docs.docker.com/desktop/setup/install/windows-install/

a) Enable *Use WSL 2 instead of Hyper-V and **<ins>do not enable</ins>** "Allow Windows Containers".
<p align="center">
   <img src="./img/00_install_options.png" width="600" />
</p>  
