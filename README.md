## For Mac OS

#### Declaration

This repository is deprecated in 2023.06 and only used for computer group assignment. If there is any offense, please contact us for deletion.

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

5. After everything is done, double click “run.command”, then you can finish the study.