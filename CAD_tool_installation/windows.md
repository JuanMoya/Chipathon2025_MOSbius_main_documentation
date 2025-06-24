# Installation Steps for Windows

The Docker image used in this 2025 Chipathon is pre-packaged Docker container provided for 2025 Chipathon provided by Harald Pretl's lab **IIC-OSIC-TOOLS**: https://github.com/sscs-ose/sscs-chipathon-2025/tree/main/resources/IIC-OSIC-TOOLS

First, a block diagram with the main installation steps:
<p align="center">
   <img src="./img/Installation_flow.png" width="600" />
</p>  

GUI-based tool setup:

1) Assuming that you have installed on your Windows machine **<ins>Windows Powershell</ins>**:

   a) Create a folder where you will pull Harald Pretl's Docker image.

   b) Clone 2025 Chipathon Docker image from: https://github.com/sscs-ose/sscs-chipathon-2025/tree/main/resources/IIC-OSIC-TOOLS with the following command:
  ```
  git clone https://github.com/sscs-ose/sscs-chipathon-2025.git
  ```
<p align="center">
   <img src="./img/cloned_repo.png" width="600" />
</p>  

2) Download Docker: https://docs.docker.com/desktop/setup/install/windows-install/

Enable *Use WSL 2 instead of Hyper-V and **<ins>do not enable</ins>** "Allow Windows Containers".
<p align="center">
   <img src="./img/00_install_options.png" width="600" />
</p>  

3) Go to the local folder where the Docker image was cloned. Then, enter the  **IIC-OSIC-TOOLS** folder and run the following command:
  ```
  .\start_x.bat
  ```
There are two other scripts that can be run based on your preferences, as indicated in:

https://github.com/sscs-ose/sscs-chipathon-2025/blob/main/docs/install_instructions/Windows/install_docker_desktop.md

After the command finalizes pulling the image, it is possible that the tagged image downloaded is **latest** instead of **chipathon**, as observed in the figure below.
<p align="center">
   <img src="./img/tag_latest.png" width="600" />
</p>  

This is because in the start_x.bat file, the tag image is **latest** as indicated below:
<p align="center">
   <img src="./img/bat_latest.png" width="600" />
</p>  

Modify the line and include **chipathon** instead of **latest**. Go to the Docker application and erase both container and image associated with **IIC-OSIC-TOOLS**.

Run again the command:
  ```
  .\start_x.bat
  ```

Now, the pulled image should be correct as indicated below:
<p align="center">
   <img src="./img/tag_chipathon.png" width="600" />
</p>  
