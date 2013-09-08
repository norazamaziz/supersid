SuperSID on Windows
===================

Version 1.2 is available with a Windows installer. This package installs all necessary dependencies, including a running library for Python.

If you want to use this version, you need to install the necessary envrionment first:
 - Download and install Python from the official [Python site](http://python.org) matching your Windows version. [version 2.7 or 3.3]
 - Download and install PyAudio from http://people.csail.mit.edu/hubert/pyaudio/#downloads matching your Python and Windows version
 - Download and install the matplotlib package matching your Python and Windows version
	- Requires numpy, dateutil, pytz, pyparsing, six:
	- Go to http://www.lfd.uci.edu/~gohlke/pythonlibs/
	- Download and install them (choosing the packages matching your Python and Windows version)


Here are the programs for a Windows 32bits and Python 3.3:
31-Aug-2013  05:00 PM        20,238,336 python-3.3.2.msi
31-Aug-2013  04:49 PM           356,332 pyaudio-0.2.7.py33.exe
31-Aug-2013  04:48 PM         5,861,646 matplotlib-1.3.0.win32-py3.3.exe
03-Sep-2013  10:28 PM           310,746 python-dateutil-2.1.win32-py3.3.e
03-Sep-2013  10:29 PM           719,292 pytz-2013b.win32-py3.3.exe
03-Sep-2013  10:29 PM           198,188 six-1.4.1.win32-py3.3.exe
03-Sep-2013  10:30 PM           226,588 pyparsing-2.0.1.win32-py3.3.exe
03-Sep-2013  10:34 PM        11,453,891 numpy-MKL-1.7.1.win32-py3.3.exe

As you can notice, **wxPython** is absent as not yet ported on Python 3.

Once the environment is setup, fetch the application:
 - You can simply go to https://github.com/ericgibert/supersid and click on the "Download ZIP" button
**OR**
 - You can first install Git on Windows: http://msysgit.github.io/
	- I have installed: Git-1.8.3-preview20130601.exe
 - Then issue the command: ````git clone https://github.com/ericgibert/supersid.git````
 - In the future, move to *supersid* directory and issue the command ````git pull```` to download the latest updates

The application runs nevertheless very well in text mode.

In the Config\supersid.text.cfg file:
 - Text mode declaration
 - Change the data_path to a Windows target directory
 - Choose a name for your site

````
	[PARAMETERS]
	viewer=text
	site_name = CHEZMOI
	data_path = C:\Documents and Settings\eric\My Documents\supersid\Data
````

then call ````supersid\supersid.py Config\supersid.text.cfg````