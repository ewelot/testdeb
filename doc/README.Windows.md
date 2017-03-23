
# README.Windows

The following instructions are intended to guide you on setting up
a virtual Linux operating system which can run on any computer.
This system can then be used to install and test the [AIRTOOLS]
(https://github.com/ewelot/airtools) software
without interfering with your own host operating system.


1. Install VirtualBox
Download and install the [VirtualBox](http://www.virtualbox.org).
Choose the version which fits your operating system.
In addition you should also download and install the VirtualBox
Extension Pack.


2. Download a Linux Live-DVD
Get a current Live-DVD ISO image file of a supported Linux distribution.
I highly recommend the XUbuntu distribution which you can find at:
    https://xubuntu.org/getxubuntu/
Choose a mirror download for latest LTS release and get the 64bit ISO image.


3. Create a virtual machine
Start the VirtualBox software. It opens a new window from which you create
and manage your virtual machines (VM). In short, a VM is a virtual computer
running on virtual hardware provided by the VirtualBox software.
Create a new VM:
  - choose name, e.g. xubuntu-live
  - choose a memory size of at least 2GB
  - choose to not add a virtual disk (not required for basic work)
Make the ISO file available to the VM:
  - modify settings of the VM, open the "Storage" tab
  - select empty CDROM entry and click the right-most CDROM icon
  - browse and select the ISO image file
Other tweakings:
  - on "System" tab make sure booting from optical media is enabled
  - on "System" / "Processor" tab increase number of CPU to about half the
    number of your physcal CPU's
  - on "Display" tab increase video memory to 32MB
  - on "USB" tab activate USB-2.0 or USB-3.0


4. Boot Linux from Live-DVD
Start booting your VM. You can choose your prefered language und start the
live system (do not install it).
Note on XUbuntu Linux: the application menu is activated by the top-left
icon. The shutdown-button is located on that menu at bottom right position.


5. Installing airtools
Follow instructions from the [INSTALL](INSTALL.md) file.


6. Making your FITS image files available to Linux
Copy your images to an external USB disk (or pen drive). Plug-in the device
on your host computer. Hand over the device to the VM by using the VM menu
"Devices/USB".


7. Saving your work
Please note that any file modifications inside of this running Linux
system are not persistent and lost when you shut down the live system.
This is fine as long as you are evaluating/testing the software. For real
work however it is necessary to save your processed data, e.g. by copying
to an external USB disk.


8. Permanent Linux installation
If you find the AIRTOOLS software useful and you intend to use it regularly
then it is recommended to install the Live-DVD content to a virtual disk
and boot from this device. A subsequent installation of the airtools software
and all further file modifications will be permanent and visible upon next
boot of the VM.

