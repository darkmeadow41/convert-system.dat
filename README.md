# Convert system.new.dat
Simple approach to convert system.newdat to img on Ubuntu 14.04 and above

What we need: 
  1. Android version 6-8 rom of course
  2. Python file to convert
  
Lets do it:
  1. We unpack archive with firmware in any folder (for example, in rom): 

  $ mkdir ~ / rom 

  $ cd ~ / rom 
  $ wget https://github.com/xpirt/sdat2img/raw/master/sdat2img.py 
  Run the script: 

  $ chmod + x sdat2img.py 
  $ ./sdat2img.py system.transfer.list system.new.dat system.img 
  It converts the system.new.dat file into a raw image named system.img.  Mount the image to the mnt subfolder: 

  $ mkdir mnt 
  $ sudo mount -t ext4 -o loop system.img ~ / rom / mnt 


Android directory structure 

After unpacking the system, the following directory structure will appear: 
