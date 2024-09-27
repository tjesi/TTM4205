# Installing - Extra notes (for Windows, Linux and Mac)
* Remember to update the git repository chipwhisperer to the latest version to get the correct firmware.
* Always check that the paths to firmware are correct when running the labs. Depending on your install they might not be.
* If you are on Windows, remember to turn off WSL.
* If you are having trouble with the SAM4S target board switch to the STM32F4 target board (in a big plastic bag in the lab)
* If you have any questions post on the Ed Forum.


## Mac and Linux only
You should be able to run a standalone version of this lab using the firmware provided [here](../CW/2024/firmware.zip) and the lab notebooks folder found [here](../CW/2024/CW.zip).

## String replacements in an entire folder

Replacing paths in every single file in all your notebooks can be a lot of work. Here is a shell function you can put into you .zshrc or .bashrc (or the shell config/script file you are currently using). If you don't know which shell you use, the default is in most cases bash, but you can check using the command `echo $0`.

#### The function for replacing strings in all files in a folder 

```
srepl() {
    local searchword=""
    local replaceword=""
    local startfolder="."

    # Function to show usage
    local usage() {
        echo "Usage: srepl -s searchword -r replaceword [-f startfolder]"
        echo "  -s    Search word"
        echo "  -r    Replace word"
        echo "  -f    Start folder (optional, default is current directory)"
        return 1
    }
    # Escape special characters for sed
    local escape_for_sed() {
        echo "$1" | sed -e 's/[\/&]/\\&/g'
    }

    # Parse command-line options
    while getopts "s:r:f:" opt; do
      case $opt in
        s) searchword=$(escape_for_sed "$OPTARG") ;;
        r) replaceword=$(escape_for_sed "$OPTARG") ;;
        f) startfolder=$OPTARG ;;
        *) usage ;;
      esac
    done

    # Check mandatory options
    if [ -z "$searchword" ] || [ -z "$replaceword" ]; then
        echo "Error: Search and replace words are mandatory."
        usage
	return 1
    fi

    # Execute the find and sed command
    find "$startfolder" -type f -exec sed -i -e "s/$searchword/$replaceword/g" {} \;

    echo "Replacement complete."
    return 0
}
```

#### How to use the `srepl` function:

Replace string "../../../hardware/victims/firmware" with "../../../firmware/mcu":

```
srepl -s "../../../hardware/victims/firmware" -r "../../../firmware/mcu"
```


# Installing Chipwhisperer on Windows
*Based on https://chipwhisperer.readthedocs.io/en/latest/windows-install.html by newae*

## 1 WSL and Bash
There have been reported some problems with Windows Subsystem for Linux (WSL) and some of the tools needed for the chipwhisperer lab. These issues seems to be related to the `%%bash` blocks in jupyter. If you get any errors regarding `make`, or any Linux distribution, try disabling WSL or changing `%%bash` to `%%sh`. When testing I (Caroline) did not need WSL installed at all in order to complete the lab.

## 2 Windows long file path
It is recommended to enable long paths on Windows to prevent any files from not being copied during installation of Chipwhisperer.

To enable long paths, open the Local Group Policy editor by pressing `Win + R`, typing `gpedit.msc` and pressing `Return`. Navigate then to `Computer Configuration > Administrative Templates > System > Filesystem` and double click `Enable Win32 long paths`. It should look like the image below. When this is done you need to restart the computer.

![gpedit.msc screenshot](img/windows_long_path.png)

## 3 Download Chipwhisperer setup executable
You can download [Chipwhisperer.v5.7.0.Setup.64-bit.exe](https://github.com/newaetech/chipwhisperer/releases/download/5.7.0/Chipwhisperer.v5.7.0.Setup.64-bit.exe) [here](https://github.com/newaetech/chipwhisperer/releases/download/5.7.0/Chipwhisperer.v5.7.0.Setup.64-bit.exe), or you can find the link from newaetech's github release page [here](https://github.com/newaetech/chipwhisperer/releases).

Once the setup executable is downloaded, run it and choose install path. Remember you need to have read/write permissions in the install location, so if using a lab computer avoid installing it in `C:Program Files`. I recommend installing it in your user home directory (default). Follow the setup wizard's recommended installation. I also recommend to tick the box to create a desktop shortcut.

## 4 Running ChipWhisperer
Once the above is completed, running the new `ChipWhisperer.exe` program you installed in the previous step should open a jupyter notebook in your browser. If you didn't tick the `Create a desktop shortcut` box, this should be found in `C:\Users\<username>\ChipWhisperer5_64` if you followed the setup wizard recommended install path.

## 5 Opening the premade lab notebooks
The easiest way to open the lab notebooks is to download the zip file containing the lab notebooks [here](../CW/2024/CW.zip) unzip the files, and place them inside the chipwhisperer jupyter folder located in `C:\Users\<username>\ChipWhisperer5_64\cw\home\portable\chipwhisperer\jupyter`. They should then show up in your jupyter notebook in the browser. You might need to restart `ChipWhisperer.exe` before this takes effect.

## 6 Completing the ChipWhisperer Lab
You are now ready to take on the lab tasks.


# Installing Chipwhisperer on linux
See [Chipwhisperer linux installation](https://chipwhisperer.readthedocs.io/en/latest/linux-install.html) for details on different installation methods.

## Required packages
Update packages:
```
sudo apt update && sudo apt upgrade
```
Installing prerequisites:
```
sudo apt install build-essential gdb lcov pkg-config \
    libbz2-dev libffi-dev libgdbm-dev libgdbm-compat-dev liblzma-dev \
    libncurses5-dev libreadline6-dev libsqlite3-dev libssl-dev \
    lzma lzma-dev tk-dev uuid-dev zlib1g-dev curl
```
Prerequirsites for building firmware for targets
```
sudo apt install libusb-dev make git avr-libc gcc-avr \
    gcc-arm-none-eabi libusb-1.0-0-dev usbutils
```

## Python
I recommend using either [miniforge/conda](https://github.com/conda-forge/miniforge) or [pyenv](https://github.com/pyenv/pyenv) for managing your python environments.

## Installing chipwhisperer
Start by grabbing ChipWhisperer from Github. Install wherever you like, but the code below will download it to your home directory:
```
cd ~/
git clone https://github.com/newaetech/chipwhisperer
cd chipwhisperer
git submodule update --init jupyter # grab Jupyter notebook tutorials
```
Next, we’ll need to make some udev rules so that we have permission to access USB and serial devices. ChipWhisperer includes a default set of rules that give you access to NewAE USB devices:

```
sudo cp hardware/50-newae.rules /etc/udev/rules.d/50-newae.rules
sudo udevadm control --reload-rules
```
Those rules actually give permission to the chipwhisperer group, so you’ll need to create that group and add your user to that group:

```
sudo groupadd -f chipwhisperer
sudo usermod -aG chipwhisperer $USER
sudo usermod -aG plugdev $USER
```
Make sure you restart your computer after this step.

### Note
Older install instructions used the plugdev group, which is created by default on some distros and not on others. These install instructions instead use a dedicated chipwhisperer group, so if you’ve installed chipwhisperer before and want to update to a new rules file, make sure you create the chipwhisperer group.

With that done, all that’s left is to install ChipWhisperer:
```
python -m pip install -e .
python -m pip install -r jupyter/requirements.txt
```
You may also want to grab nbstripout, which will make git and jupyter interact a little nicer:

```
cd jupyter
pip install nbstripout
nbstripout --install # must be run from the jupyter folder
```
