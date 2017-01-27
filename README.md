MD380tools VM for VirtualBox
Warren Merkel, KD4Z

Current Version: 3.08 (after you glv)
Image file updated:	 01/04/2017  Version 3.0
Installation PDF updated: 01/14/2017

From github project
https://github.com/KD4Z/md380tools-vm

Follow the installation directions in the PDF found here:

https://github.com/KD4Z/md380tools-vm/raw/master/MD380tools_VM_installation_3.06.pdf

You do not need to download any files list here on this github site, except the install pdf above!


You DO need to download the image from links below if you are not on version 3.x
Don't download from these links if you already have version 3.x!  The 3.0 VM self updates
to the lastest version found in this github site every time that you run glv. 

If you are still running version 2.x of this VM, you should upgrade to 3.0 to avoid
issues that have already been resolved.

This project allows you to create the latest firmware for the MD-380 / MD-390
series of radios from Tytera (TYT).  It leverages the MD380tools project by
Travis Goodspeed found elsewhere on github.  It also downloads the dmr-marc contact
database into the radio.

This VM provided in the image provides simple single-word menu that is easy to
use, and does all of the heavy lifting of installing the MD380tools project files.
 
The most important benefit of using this VM instead of other solutions is you can 
update radio firmware and user contact data while offline from the Internet.  Run
one single command (glv) while online, and then you can disconnect your laptop, 
and take it where you dont' have a live internet connection.  

If you are interested in adding in private DMR IDs to the user contact data, support
for that has been recently added.  This feature may also be interesting to you if
use a hotspot device and are annoyed that certain parts of the contact database 
now show up with blank, redacted location data.

Other interesting tweaks in this VM make it stand out as being better than just
the results from running the base md380tools scripts.

Be sure to read it completely before emailing questions!  99% of all questions are
answered in the installation PDF.   Consider joining the BrandMeister DMR talkgroup
3148 Facebook group for assistance from others, and lots of information. 
Link:  https://www.facebook.com/groups/158270421244005/

European users have access to this Facebook group, specializing in Dutch,
though English posts are welcome:
https://www.facebook.com/groups/105977523245213
courtesy of PD0DIB. 

You will need to download the VirtualBox Appliance image file from these links:

Single Image (Zip):
https://drive.google.com/file/d/0Bwoi2MrlPb3vVEt3Ym4tVHF3SDQ/view?usp=sharing
	
Use one of the above links, or the 4 links below.  Don't do both!
	
Parts - Must use 7-zip to extract  http://www.7-zip.org/download.html	
	
Part 1: https://drive.google.com/file/d/0Bwoi2MrlPb3vY2hkb0lVZ3Z4R3c/view?usp=sharing
Part 2: https://drive.google.com/file/d/0Bwoi2MrlPb3vMDlCMmY2V0FWY28/view?usp=sharing
Part 3:	https://drive.google.com/file/d/0Bwoi2MrlPb3vTFZfRGZ4X3NJakU/view?usp=sharing
Part 4: https://drive.google.com/file/d/0Bwoi2MrlPb3vSHkwdHV1dGVaZjA/view?usp=sharing

For the parts, download each one.  You will need to use the 7-zip program to extract them
back into the original OVA Appliance file.
 
Install 7-Zip, and then Right-Click on the first part file and find the 7-Zip menu, and
follow it out to extract.

** Optional Image for VMware **
User videobuff provided a converted image file, more suitable for 
VMWare Fusion users: In case you wish to install a ready-to-go VMWare container,
you can download it here.  (This is the full image):

https://drive.google.com/open?id=0BwED_-BHnZjSWklsNjY3VHBqMVE

-OR Download the VMWare image in parts - don't download these if you download from the single link above.

Parts - Must use 7-zip to extract  http://www.7-zip.org/download.html	

Part 1:	https://drive.google.com/file/d/0BwED_-BHnZjSdERwY1BHc1Y3ekk
Part 2: https://drive.google.com/open?id=0BwED_-BHnZjSYnZEeXJHcjh5R3c
Part 3: https://drive.google.com/open?id=0BwED_-BHnZjSb3NzSE41azhzN3M
Part 4: https://drive.google.com/open?id=0BwED_-BHnZjSNmlOMTJvT3l4VWM

For the parts, download each one.  You will need to use the 7-zip program to extract them
back into the original OVA Appliance file.

Noteable features:

  Simple, one word commands.   (It's really easy!)
  
  Runs under Windows or OS-X hosts using the free VirtualBox host software.  Runs under
  VMware as well.  Use the Optional Image mentioned above.
 
  Able to update radios when not connected to the internet, great for laptops.

  Able to add private DMR IDs to the UsersCSV using a local fixed file, or can FTP in
  a static file on the fly.

  Automatically adds back some missing userCSV data from the EU using static seed file

  Automatically stays updated with changes going forward. You will not need to download
  the VM Image again, after getting to Version 3.0, the glv command will self update all
  portions of the VM.

  Able to update firmware on MD-380 and MD-390 radios with GPS

  Multiple language support.   Currently 3 alternate languages are supported.
  
  Dutch			(enable with:  touch lang.nl )  Courtesy of PD0DIB 
  Portuguese	(enable with:  touch lang.pt )  Courtesy of CS7AGH
  Italian		(enable with:  touch lang.it )  Courtesy of IW0QPP
  
   
  If you can help translate into other languages, create a branch, and modify the
  "strings" script (found here), and request a pull.  Or send me the new language section in email.  

  Able to display user's first name in the nickname space, which makes the name easy to see.
  
  User customization ability using your own bash scripting.  Callouts to user scripts are available
  prior to glv, during filtering, and after glv is completed.  Knock yourself out!
  
  KD4Z