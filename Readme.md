## macOS (OS X) ISO Creator ##
Create bootable ISO images of macOS or OS X from .app installers.
## Support for the following OS ##
+ 10.9
+ 10.10
+ 10.11
+ 10.12
+ 10.13
## Options ##
	Optional Flags:
		-h: Display this dialog
		-c: Create flag to initiate ISO creation.
		-d: Enable Debugging.
	Required Flags:
		-s absolute_path: Source file absolute path.
## Examples ##
1. Create an installer from OS X Mavericks:

`./macos-iso-creator -c -s "/Applications/Install OS X Mavericks.app"`

Output: 
```
Starting Creation process for /Applications/Install OS X Mavericks.app
Working out of /tmp/creator.sh-1510187298...
/dev/disk3          	Apple_partition_scheme
/dev/disk3s1        	Apple_partition_map
/dev/disk3s2        	Apple_HFS                      	/private/tmp/creator.sh-1510187298/install_app
...............................................................................................................................................................
created: /tmp/creator.sh-1510187298/Mavericks.cdr.dmg
/dev/disk5          	Apple_partition_scheme
/dev/disk5s1        	Apple_partition_map
/dev/disk5s2        	Apple_HFS                      	/private/tmp/creator.sh-1510187298/install_build
	Validating target...done
	Validating source...done
	Retrieving scan information...done
	Validating sizes...done
	Restoring  ....10....20....30....40....50....60....70....80....90....100
	Remounting target volume...done
"disk3" unmounted.
"disk3" ejected.
"disk5" unmounted.
"disk5" ejected.
Reading Driver Descriptor Map (DDM : 0)…
Reading Apple (Apple_partition_map : 1)…
Reading disk image (Apple_HFS : 2)…
...............................................................................................................................................................
Elapsed Time: 34.909s
Speed: 209.6Mbytes/sec
Savings: 0.0%
created: /tmp/creator.sh-1510187298/Mavericks.iso.cdr
Your ISO is ready for deployment at /tmp/creator.sh-1510187298/Mavericks.iso
```
