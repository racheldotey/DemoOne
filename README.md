# Transcript-DemoOne
A test run of Python to JavaScript conversion using Transcrypt.  
Just getting a basic hello world up and running to test Transcrypt.



## Software Install

### Web Server
MAMP OR WAMP OR XAMPP are all good options

MAMP (OSX) - https://www.mamp.info/en/  
XAMPP (OSX, Windows, Linux) - https://www.apachefriends.org/index.html

### Java Developer Kit
Us the downloadable installer here:  
https://www.oracle.com/technetwork/java/javase/downloads/index.html

### Python
Use the downloadable installer here:  
https://www.python.org/downloads/

**Warning:**  
Transcrypt requires Python 3.5 or 3.6. _Python 3.7 is not yet supported._

To check your current version of Python open Terminal on MacOSX and use the following command:
```bash
python3 --version
```

**Note**  
Python provides an alies to allow multiple versions to be used on a single macheine. Consequently the latest version of Python >v3.0 can be executed via the `python3` alies. `python` will still refer to ealier (<v3.0) versions of Python if they are installed.

Additionally packages installed using easy_install or PIP can be referenced by using the `python3` alias and `-m` for module. For example:
```bash
python3 -m <package name> <command(s)>
```

### PIP
A PIP and VirtualEnv installation tutorial _(recommended by Transcrypt)_ is available here:  
https://www.dabapps.com/blog/introduction-to-pip-and-virtualenv-python/

**Condensed Install Instructions**
```bash
sudo python3 -m easy_install pip
```

To guarentee you have the latest version of PIP installed, run the upgrade method:
```bash
python3 -m pip install --upgrade pip
```
Python 3.6 uses PIP v18.0 _as of this writing._

**Note**  
PIP provides an alies to allow multiple versions of Python to be used on a single machiene. Consequently PIP commands can be executed via either `python3 -m pip` OR by `pip3`. For example the previous update command can also be triggered by the following script:
```bash
pip3 install --upgrade pip
```

#### Useful PIP Commands
View informattion about a installed package:
```bash
pip3 show <package name>
```

Upgrade an installed package:
```bash
pip3 install --upgrade <package name>
```

Uninstall a package:
```bash
pip3 uninstall <package name>
```

### VirtualEnv
A PIP and VirtualEnv installation tutorial _(recommended by Transcrypt)_ is available here:  
https://www.dabapps.com/blog/introduction-to-pip-and-virtualenv-python/

**Condensed Install Instructions**
```bash
pip3 install virtualenv
```

To guarentee you have the latest version of VirtualEnv installed, run the upgrade method:
```bash
pip3 install --upgrade virtualenv
```
Python 3.6 and PIP v18.0 use VirtualEnv v16.0 _as of this writing._


#### Useful VirtualEnv Commands
Create a new virtual enviroment:
```bash
cd ~/code/myproject/
python3 -m virtualenv env
```

Activate your new virtual enviroment:
```bash
source env/bin/activate
```
_The active enviroment resets when Terminal is closed._

Deactivate your current virtual enviroment (sets it back to global):
```bash
deactivate
```

Verify which enviroment is active:
```bash
which python3
```

### Transcrypt
https://www.transcrypt.org

First go to your project folder:
```bash
cd ~/code/myproject/
```

Then activate your projects virtual enviroment:
```bash
source env/bin/activate
```

Finally install Transcrypt into that enviroment:
```bash
pip3 install transcrypt
```

#### Useful Transcrypt Commands
Create a new virtual enviroment:
```bash
cd ~/code/myproject/
transcrypt -b index.py
```

For more Transcript build command optiomns us the `-h` command:
```bash
transcrypt -h
```
OR see the following link: https://www.transcrypt.org/docs/html/installation_use.html
