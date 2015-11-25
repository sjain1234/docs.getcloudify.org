---
layout: bt_wiki
title: Installing Cloudify
category: Intro
publish: true
pageord: 200
---

To start using Cloudify, you must first install it.


# Installing using premade packages

Currently, packages are distributed for Centos 6.5 and 7, RHEL 7 and Windows.

## Windows

To install on Windows:

* Download the installer from the [Downloads page](http://getcloudify.org/downloads/get_cloudify_3x.html) corresponding with the version you would like to install.
* Run the executable installer.
* Follow the installation instructions.
* When the installation is finished, double click the new Cloudify icon on your desktop.

After the installation is complete, try running `cfy -h` in your terminal.


## Linux

To install via rpm packages, you must have Python2.7.x and pip 1.5+ installed and Python2.7.x must be executable as `python` from the path.

### Centos/RHEL

* Download the installer from the [Downloads page](http://getcloudify.org/downloads/get_cloudify_3x.html) corresponding with the version you would like to install.
* Open a terminal at the directory where you downloaded the file.
* Run (replacing `<pkg.rpm>` with the path to the file you downloaded):

{{< gsHighlight  bash  >}}
sudo rpm -i <pkg.rpm>
source /opt/cfy/env/bin/activate
{{< /gsHighlight >}}

After the installation is complete, try running `cfy -h` in your terminal.


# Installing using an installation script

A script is supplied for you to install Cloudify on Linux, Windows and OS X.

## Prerequisites

To install using the script, you must have Python 2.7.x preinstalled.

{{% gsWarning title="Prerequisites Installation" %}}
By default, this script will not install any prerequisites (like pip, or any required compilers). You can supply it with the `--force` flag which will install all prerequisites without prompting you for anything other than a sudoer password (if required).
{{< /gsHighlight >}}

Note that the script requires an internet connection.

Run `python get-cloudify.py -h` for additional information.


## Installation

You can download the script from [here](#){: .openRegisForm}

Then, run `sudo python get-cloudify.py` on Linux or OS X and `python get-cloudify.py` on Windows.

After the installation is complete, try running `cfy -h` in your terminal.

{% include  download_py_script_tracking.html %}


That's it! Cloudify is installed. You can now try using it to [deploy your first application](intro-getting-started.html).