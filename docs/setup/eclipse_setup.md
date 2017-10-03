## Install Eclipse
* Install eclipse IDE from eclipse.org
* Install python plugin for eclipse:  http://pydev.org/updates
* Preq-installation: java JRE and JDK
* Install NOKIA RED plugin for Eclipse: http://master.dl.sourceforge.net/project/red-robot-editor/repository
  * https://github.com/nokia/RED
* Install Python 3 for MAC:
  * Install from python.org using .dmg file
* Configure Python Virtual Enviroment:
  1.  Install python virtual enviromment: 
    -  pip3 install virtualenv
  2. Create python 2.7 or python 3.6 environment:
    - virtualenv -p <python-version> <desired-path>
    - virtualenv -p /usr/bin/python2.7 python27env
    - virtualenv -p /Library/Frameworks/Python.framework/Versions/3.6/bin/python3.6 python36env
  3. Activate/Deactivate python virtual env:
    - source python36env/bin/activate
    - deactivate
* Configure Eclipse to Switch between python version:  
    Window -> Preferences -> Robot Framework -> Installed Frameworks
  
