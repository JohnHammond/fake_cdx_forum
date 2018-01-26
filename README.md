__www.uscga.bluenet__
==========

> John Hammond | June 20, 2016 
> _Last Updated June 20, 2016_

-----------------------------------------------------------------

__Running the Web Server__
----------------

One of the prevailing mindsets we have as a team for [CDX] 2017 is to _play to the rules..._ and _only_ the rules. It has been come too clear that the victors of [CDX] win because they _game_ the _game_; they create an unrealistic network that only serves the purpose of scoring points and making it on the board.

So; we'll play along.

With that in mind, here is what I cooked for the required web server: [`index.html`][1]. It is a stand-alone file, that I envision should be served up by simply...

```
python -m SimpleHTTPServer
```

... because it needs nothing else.

The Rules
-------

For [CDX] 2016, a Bluenet's web server had to follow the below criteria. For each section, I have noted that this [`index.html`][1] does meet the requirement -- denoted by an `(X)` -- and I've __bolded__ the words that let me get away with it.

> Each Blue Cell website must provide a __dynamic__ `(X)` message board  or "forum", __linked from the front page of the site__ `(X)`, meeting the following critera:
> 
> 
> * The message board must be “threaded,” collecting posts into threads or topics for convenient reading. `(X)`
> 
> *   Users must have the ability to __create new threads__ `(X)`, __post to existing threads__ `(X)`, __edit or delete their own existing posts__ `(X)`, __quote text from earlier posts__ `(C)`, and __define signature blocks that will automatically be appended to their posts__ `(X)`. 
> 
> *  Users must __be able to embed hyperlinks and images into their posts, and must be able to use standard HTML markup to format their posts.__ `(X)`
>     -  _The users can put any content they would like in their posts._
>
> *  Users must be able to create personal profiles, to __include at least a full name, email address, personal web site URL, and personal description.__ `(X)`
> 
> * Users must have the ability to upload and download files to the forums. __In particular, users must have the ability to upload “avatar” images that will be automatically displayed as part of their own posts.__ `(X)`
> 
> * At a minimum, the board must have two sections titled Customer Support and Public Discussion, in which any user on the BLUENET or SIMNET may participate. At their own discretion, Blue Cell teams may create additional sections with more limited access. `(X)`
> 
> * The board __may__ require user registration and password authentication before granting posting access. If so, a new user must be able to register without requiring any action on the part of the Blue Cell team. The user registration process may include automated methods for verifying an applicant’s legitimacy (i.e., verification of an email address, a CAPTCHA code, and so on). `(X)`
> 
> * Users must be able to recover their account passwords if forgotten, without requiring any action on the part of the Blue Cell team. `(X)`
>     - _Without any registration, there is no password to be recovered; but I offer this 'functionality' anyway because it is apparently required regardless_
>  


----

And that's all that it needs. Nowhere does it specify it needs to be running server-side code, or with a database, or any of that nonsense... it only needs to be, "dynamic": which I can pull off with [JavaScript].

Everything runs on the client browser; so there should be no explicit web vulnerabilities in our webpage itself.


[1]: index.html
[CDX]: https://www.nsa.gov/public_info/press_room/2014/cdx_media_advisory.shtml
[Samba]: https://www.samba.org/
[Ubuntu Server]: http://www.ubuntu.com/server
[Citadel]: http://www.citadel.org/doku.php
[Active Directory]: https://en.wikipedia.org/wiki/Active_Directory
[Domain Controller]: https://en.wikipedia.org/wiki/Domain_controller
[git]: https://git-scm.com/
[FTP]: https://en.wikipedia.org/wiki/File_Transfer_Protocol
[SSH]: https://en.wikipedia.org/wiki/Secure_Shell
[Cowrie]: https://github.com/micheloosterhof/cowrie
[read-only]: https://wiki.samba.org/index.php/Join_a_domain_as_a_RODC
[hMail]: https://www.hmailserver.com/
[Windows]: https://www.microsoft.com/en-us/windows
[FileZilla]: https://filezilla-project.org/download.php
[Linux]: https://en.wikipedia.org/wiki/Linux
[time skew]: http://windowsitpro.com/security/q-why-time-synchronization-between-windows-machines-critical-active-directory-ad-environmen
[DNS]: https://en.wikipedia.org/wiki/Domain_Name_System
[hypervisor]: https://en.wikipedia.org/wiki/Hypervisor
[VMWare ESXi]: https://www.vmware.com/products/esxi-and-esx/overview
[ESXi]: https://www.vmware.com/products/esxi-and-esx/overview
[RAM]: https://en.wikipedia.org/wiki/Random-access_memory
[hard drive]: https://en.wikipedia.org/wiki/Hard_disk_drive
[CPU]: https://en.wikipedia.org/wiki/Central_processing_unit
[processor]: https://en.wikipedia.org/wiki/Central_processing_unit
[IP address]: https://en.wikipedia.org/wiki/IP_address
[ESXi Shell]: https://pubs.vmware.com/vsphere-50/index.jsp?topic=%2Fcom.vmware.vcli.migration.doc_50%2Fcos_upgrade_technote.1.4.html
[SSH]: https://en.wikipedia.org/wiki/Secure_Shell
[ssh]: https://en.wikipedia.org/wiki/Secure_Shell
[virtual machine]: https://en.wikipedia.org/wiki/Virtual_machine
[virtual machines]: https://en.wikipedia.org/wiki/Virtual_machine
[VM]: https://en.wikipedia.org/wiki/Virtual_machine
[VMs]: https://en.wikipedia.org/wiki/Virtual_machine
[command-line]: https://en.wikipedia.org/wiki/Command-line_interface
[command line]: https://en.wikipedia.org/wiki/Command-line_interface
[cli]: https://en.wikipedia.org/wiki/Command-line_interface
[GUI]: https://en.wikipedia.org/wiki/Graphical_user_interface
[graphical user interface]: https://en.wikipedia.org/wiki/Graphical_user_interface
[PowerCLI]: https://www.vmware.com/support/developer/PowerCLI/
[PowerShell]: https://en.wikipedia.org/wiki/Windows_PowerShell
[cmdlet]: https://msdn.microsoft.com/en-us/library/ms714395(v=vs.85).aspx
[cmdlets]: https://msdn.microsoft.com/en-us/library/ms714395(v=vs.85).aspx
[iso]: https://en.wikipedia.org/wiki/ISO_image
[.iso]: https://en.wikipedia.org/wiki/ISO_image
[operating system]: https://en.wikipedia.org/wiki/Operating_system
[Copy-DatastoreItem]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI55/html/Copy-DatastoreItem.html
[datastore]: https://pubs.vmware.com/vsphere-4-esx-vcenter/index.jsp?topic=/com.vmware.vsphere.server_configclassic.doc_41/esx_server_config/introduction_to_storage/c_datastores.html
[datastores]: https://pubs.vmware.com/vsphere-4-esx-vcenter/index.jsp?topic=/com.vmware.vsphere.server_configclassic.doc_41/esx_server_config/introduction_to_storage/c_datastores.html
[Get-Datastore]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI51/html/Get-Datastore.html
[file system]: https://en.wikipedia.org/wiki/File_system
[vmstore]: https://www.petri.com/vsphere-powercli-psdrives
[PSDrive]: https://msdn.microsoft.com/en-us/powershell/scripting/getting-started/cookbooks/managing-windows-powershell-drives
[datacenter]: https://pubs.vmware.com/vsphere-50/index.jsp?topic=%2Fcom.vmware.vsphere.introduction.doc_50%2FGUID-33954268-2492-4758-A663-6F01548B5779.html
[datacenters]: https://pubs.vmware.com/vsphere-50/index.jsp?topic=%2Fcom.vmware.vsphere.introduction.doc_50%2FGUID-33954268-2492-4758-A663-6F01548B5779.html
[Ubuntu Server]: http://www.ubuntu.com/server
[New-VM]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI55/html/New-VM.html
[Start-VM]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI41U1/html/Start-VM.html
[Stop-VM]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI41U1/html/Stop-VM.html
[Remove-VM]: https://pubs.vmware.com/vsphere-60/index.jsp?topic=%2Fcom.vmware.powercli.cmdletref.doc%2FRemove-VM.html
[Open-VMConsoleWindow]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI55/html/Open-VMConsoleWindow.html
[Firefox]: https://www.mozilla.org/en-US/firefox/new/
[Mozilla Firefox]: https://www.mozilla.org/en-US/firefox/new/
[VMware Workstation]: https://www.vmware.com/products/workstation
[Google Chrome]: https://www.google.com/chrome/browser/desktop/
[gigabyte]: https://en.wikipedia.org/wiki/Gigabyte
[hard drive]: https://en.wikipedia.org/wiki/Hard_disk_drive
[harddrive]: https://en.wikipedia.org/wiki/Hard_disk_drive
[RAM]: https://en.wikipedia.org/wiki/Random-access_memory
[Get-CDDrive]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI41U1/html/Get-CDDrive.html
[Set-CDDrive]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI41U1/html/Set-CDDrive.html
[CD drive]: https://en.wikipedia.org/wiki/Optical_disc_drive
[New-CDDrive]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI41U1/html/New-CDDrive.html
[Coast Guard Academy]: http://uscga.edu
[OnTheHub]: http://onthehub.com/
[vSphere Client]: https://my.vmware.com/en/web/vmware/info/slug/datacenter_cloud_infrastructure/vmware_vsphere/6_0
[virtual switch]: http://www.virtualizationadmin.com/articles-tutorials/vmware-esx-and-vsphere-articles/installation-and-deployment/vmware-understanding-virtual-switch.html
[New-VirtualSwitch]: https://www.vmware.com/support/developer/PowerCLI/PowerCLI41U1/html/New-VirtualSwitch.html
[vCenter Server]: https://www.vmware.com/products/vcenter-server