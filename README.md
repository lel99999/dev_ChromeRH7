# dev_ChromeRH7
Chrome Ansible Installation and Configuration for RHEL 7.x

#### Policy File Information
[Linux Quick Start](https://sites.google.com/a/chromium.org/dev/administrators/linux-quick-start)<br/>

For Linux:<br/>
Create policy json file (i.e. chrome.json) and copy to /etc/opt/chrome/policies/managed<br/>

#### Add RHEL 7 Repo for libvulkan dependency errors
```
### Addresses libvulkan.so.1 Error
$sudo /usr/bin/subscription-manager repos --enable=rhel-7-server-e4s-optional-rpms


$sudo wget https://dl.google.com/linux/direct/google-chrome-stable_current_x86_64.rpm
$sudo yum -y install redhat-lsb libXScrnSaver
$sudo yum -y localinstall google-chrome-stable_current_x86_64.rpm
```

#### Install Latest EPEL 7
```
$sudo yum install -y https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
```





