## Big Study For Mac OS

#### Declaration

This repository is deprecated in 2023.06 and only used for computer group assignment. If there is any offense, please contact us for deletion.

It can only applied to Youth Shandong. 

Thanks to all open source authors of the big study. 

#### Testing Environment

```
MacOS Ventura 13.3.1
```

#### Requirements

```py
python 3.6~3.9
Anaconda latest
openssl@1.1
urllib3==1.26.6 
```

#### Project Structure

```xml
---releaseForMac
	---config.js (store your wx openid)
	---main (nessary)
	---run.command(study deployment)
```

#### HOW TO USE

1. open your Terminal on Mac OS, install openssl with homebrew:

```
brew install openssl@1.1
```

Creating a virtual environment is recommended for package environment. But it is more convenient in your default environment of anaconda while implementing this project.

2. Install urllib3 with conda:

```
conda install urllib3==1.26.6
```

3. Change permission of file ‘run.command’ via Terminal:

```
cd releaseForMac
chmod +x run.command
```

4 .Input your openid in config.json

please refer to https://github.com/ZWN2001/big-study-doge-script to fing openid.

If you are using an ios device, it is recommended that you use an app called Stream to check your openid. In Sniff History->one History Session->click one Post query with suffix called queryPersonStudyRecord->Request->Request Body->Preview Form

5. After everything is done, double click “run.command”, then you can enjoy the study with only double click!

### NOTION:

if the solution above doesn’t work, I just upload the source code. Then you can package it yourself!

Packaging `config.json` and `main.py` into executable files that can be executed on Mac and Windows is more complicated on Mac, because the corresponding executable files need to be generated for each operating system. Here's a simple way:

To package an executable file on Mac:

1. Open the Terminal application.

2. Use the `cd` command to navigate to the directory containing `config.json` and `main.py`, making sure they are in the same directory.

3. Make sure PyInstaller is installed. If it is not installed yet, install it using the following command:

   ```shell
   pip install pyinstaller
   ```

4. In the terminal, use the following command to package `main.py` into an executable file:

   ```shell
   pyinstaller --onefile main.py
   ```

   This will generate an executable file named `main` (no file extension on Mac).

5. Place the `config.json` file in the same directory as the generated executable.

You will now generate an executable on Mac and an executable on Windows, and place the `config.json` file in the same directory as the corresponding executable. This way, you can execute the executable on different operating systems and the `config.json` file will be loaded correctly. Please note that due to packaging on different operating systems, the resulting executable may have a different file extension (none on Mac, `.exe` on Windows), this is normal.
