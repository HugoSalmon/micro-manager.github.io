---
autogenerated: true
title: Building and debugging Micro-Manager source code
layout: page
section: Programming
---

### General

-   [Micro-Manager Coding Style and
    Conventions](Micro-Manager_Coding_Style_and_Conventions "wikilink")

<!-- -->

-   [Micro-Manager Source Code](Micro-Manager_Source_Code "wikilink")

<!-- -->

-   [Using Netbeans](Using_Netbeans "wikilink") - to compile and debug
    the Micro-Manager Java layer.
-   [Using Eclipse](Using_Eclipse "wikilink") - to compile and debug the
    Micro-Manager Java layer.
-   [Using IntelliJ](Using_IntelliJ "wikilink") - to compile and debug
    the Micro-Manager Java layer

### Windows

-   [Building MM on Windows](Building_MM_on_Windows "wikilink")
-   [Visual Studio project settings for device
    adapters](Visual_Studio_project_settings_for_device_adapters "wikilink")
-   [Viewing crash dumps on
    Windows](Viewing_crash_dumps_on_Windows "wikilink") - For C++
    programmers, when all else fails

### Mac OS X and Linux

-   [Configuration options](Configuration_options "wikilink") - Build
    options on Mac OS X and Linux
-   [Debugging MM on MacOSX and
    Unix](Debugging_MM_on_MacOSX_and_Unix "wikilink") - Using gdb or
    Netbeans to debug the Micro-Manager C++ core

### Mac OS X

-   [Build on MacOS X](Build_on_MacOS_X "wikilink")
-   [Building Boost on MacOS X](Building_Boost_on_MacOS_X "wikilink")
    (obsolete)
-   [Full Build on MacOS X
    Leopard](Full_Build_on_MacOS_X_Leopard "wikilink") - How to install
    and build Micromanager 1.2 and dependencies (tested on MacOS X
    10.5.2) (obsolete)
-   [Building Universal Binaries on Mac OS
    X](Building_Universal_Binaries_on_Mac_OS_X "wikilink") (obsolete)

### Linux

-   [ArchLinux AUR
    package](https://aur.archlinux.org/packages/micromanager-git/) and
    [build
    script](https://aur.archlinux.org/cgit/aur.git/tree/PKGBUILD?h=micromanager-git&id=4b0150680d48734a8b5d7fc4cacb361caf51c64c).
-   [How To Build Micro Manager From Source On Ubuntu
    13.10](How_To_Build_Micro_Manager_From_Source_On_Ubuntu_13.10 "wikilink")
-   [Linux installation from source
    (Ubuntu)](Linux_installation_from_source_(Ubuntu) "wikilink")
-   [Linux installation from source
    (Gentoo)](Linux_installation_from_source_(Gentoo) "wikilink")
-   [Building Firewire camera support on
    Linux](Building_Firewire_camera_support_on_Linux "wikilink")
    (obsolete)
-   [Compiling MM and creating deb files on 64-bit
    Ubuntu](Compiling_MM_and_creating_deb_files_on_64-bit_Ubuntu "wikilink")
    (obsolete)

The following DeviceAdapters require dependencies to run on GNU/Linux,
some of which are packaged:

<table>
<thead>
<tr class="header">
<th><p>DeviceAdapter</p></th>
<th><p>Dependency</p></th>
<th><p>License</p></th>
<th><p>Community Package?</p></th>
<th><p>Downloadable?</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="Andor" title="wikilink">Andor</a></p></td>
<td><p>Andor SDK 2</p></td>
<td><p>? (binary library),<br />
GPL-3 (PCI driver)</p></td>
<td><p>Shell script</p></td>
<td><p>Registration required</p></td>
</tr>
<tr class="even">
<td><p><a href="AndorSDK3" title="wikilink">AndorSDK3</a></p></td>
<td><p>Andor SDK 3</p></td>
<td><p>? (binary library),<br />
? (modified BitFlow library)</p></td>
<td><p>Shell script</p></td>
<td><p>Registration required</p></td>
</tr>
<tr class="odd">
<td><p><a href="dc1394" title="wikilink">dc1394</a></p></td>
<td><p>libdc1394</p></td>
<td><p>LGPL-2.1</p></td>
<td><p>Yes</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="even">
<td><p><a href="GPhoto" title="wikilink">GPhoto</a></p></td>
<td><p>gphoto2</p></td>
<td><p>GPL-2</p></td>
<td><p>Yes</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="odd">
<td><p><a href="IDS_uEye" title="wikilink">IDS_uEye</a></p></td>
<td><p><a href="http://en.ids-imaging.com/download-ueye.html">IDS 4.30</a></p></td>
<td><p>?</p></td>
<td><p>.run installer</p></td>
<td><p>Registration required</p></td>
</tr>
<tr class="even">
<td><p><a href="OpenCVgrabber" title="wikilink">OpenCVgrabber</a></p></td>
<td><p>opencv</p></td>
<td><p>BSD</p></td>
<td><p>Yes</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="odd">
<td><p><a href="PrincetonInstruments" title="wikilink">PrincetonInstruments</a></p></td>
<td><p>libvpcam-2.7.4.2</p></td>
<td><p>? (binary library)</p></td>
<td><p>Shell script</p></td>
<td><p><a href="ftp://ftp.princetoninstruments.com/public/Software/Official/Linux/">Yes</a></p></td>
</tr>
<tr class="even">
<td><p><a href="PVCAM" title="wikilink">PVCAM</a></p></td>
<td><p>libpvcam-2.7.0.0</p></td>
<td><p>? (binary library),<br />
GPL-2 (USB-2 driver),<br />
GPL-2 (PCI driver)</p></td>
<td><p>Yes (USB),<br />
Shell script (PCI)</p></td>
<td><p><a href="ftp://ftp.princetoninstruments.com/public/Software/Official/Drivers/Linux/">Yes</a></p></td>
</tr>
<tr class="odd">
<td><p><a href="RaptorEPIX" title="wikilink">RaptorEPIX</a></p></td>
<td><p>? (XCLIB or XCAP)</p></td>
<td><p>? (<a href="http://www.epixinc.com/support/files.php">XCLIB "requires ID code"</a>)</p></td>
<td><p>.bin installer</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="even">
<td><p><a href="SpotCamera" title="wikilink">SpotCamera</a></p></td>
<td><p>SPOT SDK</p></td>
<td><p>?</p></td>
<td><p>?</p></td>
<td><p><a href="http://www.spotimaging.com/downloads.php">By request</a></p></td>
</tr>
<tr class="odd">
<td><p><a href="TISCam" title="wikilink">TISCam</a></p></td>
<td><p>uvc Kernel driver (USB)<br />
<a href="https://github.com/GNOME/aravis">aravis</a> (Gig-E)</p></td>
<td><p>GPL-2<br />
LGPL-2.1</p></td>
<td><p>N/A<br />
Yes</p></td>
<td><p>N/A<br />
Yes</p></td>
</tr>
<tr class="even">
<td><p><a href="Video4Linux" title="wikilink">Video4Linux</a></p></td>
<td><p>v4l2 Kernel driver</p></td>
<td><p>GPL-2</p></td>
<td><p>N/A</p></td>
<td><p>N/A</p></td>
</tr>
<tr class="odd">
<td><p><a href="ITC18" title="wikilink">ITC18</a></p></td>
<td><p>ITC Driver</p></td>
<td><p>?</p></td>
<td><p>?</p></td>
<td><p>By request</p></td>
</tr>
<tr class="even">
<td><p><a href="K8055" title="wikilink">K8055</a></p></td>
<td><p><a href="http://libk8055.sourceforge.net/">libk8055</a></p></td>
<td><p>GPL-2</p></td>
<td><p>Source tarball only</p></td>
<td><p>Not officially supported?</p></td>
</tr>
<tr class="odd">
<td><p><a href="MCCDAQ" title="wikilink">MCCDAQ</a></p></td>
<td><p>Unofficial <a href="ftp://lx10.tx.ncsu.edu/pub/Linux/drivers/PCI/">PCI</a> and <a href="ftp://lx10.tx.ncsu.edu/pub/Linux/drivers/USB/">USB HID</a>,<br />
Official <a href="ftp://ftp.mccdaq.com/downloads/DAQFlex/Linux/">DAQFlex USB driver</a></p></td>
<td><p>GPL-2 (Unofficial),<br />
DAQFlex EULA (Official)</p></td>
<td><p>Source tarball (Unofficial),<br />
Source tarball (Official)</p></td>
<td><p>Yes (Unofficial),<br />
Yes (Official)</p></td>
</tr>
<tr class="even">
<td><p><a href="MaestroServo" title="wikilink">MaestroServo</a></p></td>
<td><p><a href="http://www.pololu.com/catalog/product/1356/resources">UscCmd</a></p></td>
<td><p>?</p></td>
<td><p>Commandline utility</p></td>
<td><p><a href="http://www.pololu.com/file/0J315/maestro-linux-100507.media/Tar.gz">Yes</a></p></td>
</tr>
</tbody>
</table>

### Miscellaneous

-   [Free third-party tools for testing communications with
    hardware](Free_third-party_tools_for_testing_communications_with_hardware "wikilink")

{% include Programming_Sidebar text="" %}