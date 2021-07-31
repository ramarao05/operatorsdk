## operatorsdk instllation prereq in in Windows based linux Ubuntu
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
##### Windows Subsystem Linux Enable Process::
##### Open windows Power shell with admin priviliges (Task manager->File->type powershell and check the admin privilige check"
##### dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
##### Restart
##### dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
##### Restart
##### Download "https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi" and install 
##### if any permission errors , follow below steps:
##### Turn windows features on or off --> uncheck the windows virtual machine and Windows subsystem for linux and reboot machine
##### Turn windows features on or off --> check the windows virtual machine and Windows subsystem for linux and reboot machine (if the respective option available then use the above dism process)
##### For Ubuntu::
##### https://ubuntu.com/tutorials/ubuntu-on-windows#####4-install-ubuntu-for-windows-10
##### https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701?rtc=1&activetab=pivot:overviewtab
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
## operatorsdk instllation 
##### GO install v15 and above is Pre-req  (Delete any previous version before this install)
##### 1. wget https://golang.org/dl/go1.16.6.linux-amd64.tar.gz
##### 2. sudo tar -C /usr/local -xzf go1.16.6.linux-amd64.tar.gz
##### 3. export PATH=$PATH:/usr/local/go/bin
##### 4. source ~/.profile
##### 5. go version

##### Ensure GIT installed
##### 1. GOPROXY="https://proxy.golang.org|direct"
##### 2. go env | grep GOPROXY
##### 3. git clone https://github.com/operator-framework/operator-sdk
##### 4. cd operator-sdk
##### 5. git checkout master
##### 6. make install

## Software prereq:
#### Docker to work with WSL --> https://docs.docker.com/docker-for-windows/wsl/
#### DOcker as nonroot user for minikube to start --> https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user
#### Python on WSK --> https://python.plainenglish.io/setting-up-python-on-windows-subsystem-for-linux-wsl-26510f1b2d80
#### Ansible on WSL https://fakhridarmawan.medium.com/install-ansible-on-windows-subsystem-linux-ac9245219077
#### Ansible Runner on WSL https://ansible-runner.readthedocs.io/en/latest/install.html
#### Asnible runnert http ---> not sure
#### OPenshift --> https://pypi.org/project/openshift/
#### Kubectl https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/
#### minikube -> curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube




+++
Simple Process as below::

#### https://docs.openshift.com/container-platform/4.4/operators/operator_sdk/osdk-ansible.html
