# ModelSim Tutorial For Beginners

## ModelSim Installation on Windows

[Tutorial Link](https://www.youtube.com/watch?v=6-_oCSDKQEI) <br>
[Download Link](https://drive.google.com/file/d/1wBCaPRC66onO3RZL5eu-M3m_B-nsEATH/view)



<br>

## ModelSim Installation on Ubuntu

### Installation requirements

The free version of ModelSim is a 32-bit binary and therefore requires certain 32-bit libraries in order to work correctly. For Ubuntu, install the following packages

```sh
sudo dpkg --add-architecture i386
sudo apt-get update
sudo apt-get install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32ncurses6 libxft2 libxft2:i386 libxext6 libxext6:i386 
```

### Installation

Download the ModelSim - Intel FPGA edition installer (both packages) from the [Intel homepage](https://download.altera.com/akdlm/software/acdsinst/20.1std.1/720/ib_installers/ModelSimSetup-20.1.1.720-linux.run). 

Make the installer executable

```sh
chmod +x ModelSimSetup-20.1.1.720-linux.run
```

Run the installer and install ModelSim:

```sh
./ModelSimSetup-20.1.1.720-linux.run
```

We assume ModelSim to be installed to `/opt`. If this is the case, the binaries are in `/opt/modelsim_ase/bin/`. In order to work with these tools, you need to add this folder to the path variable. Therefore, add the following line to your terminal configuration file, e.g., `.bashrc` or `.zshrc`.

For `bashrc`:
```sh
export PATH=$PATH:/home/username/intelFPGA/20.1/modelsim_ase/bin
```

For `zshrc`:
```sh
export PATH="/home/username/intelFPGA/20.1/modelsim_ase/bin:$PATH"
```
or
```sh
path+=('/home/username/intelFPGA/20.1/modelsim_ase/bin')
export PATH
```
or go to `.zshrc` file and add this line in the end
```sh
export PATH="/home/username/intelFPGA/20.1/modelsim_ase/bin:$PATH"
```

Now just go to the installation path's bin directory and give command to the terminal
```sh
./vsim
```
or give command from anywhere
```sh
vsim
```
