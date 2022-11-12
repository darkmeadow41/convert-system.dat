# Convert system.new.dat
Simple approach to convert system.new.dat to img on Ubuntu 14.04 and above

What we need: 

  1. Android version 5-8 rom of course
  2. Python file to convert (sdat2img.py)
  3. Use python version 2.7
  4. Working folder to convert
  
Lets do it:

  1. First make working folder (we named "baja")
  
          mkdir baja
      
  2. Unpack rom archive and move two file name "system.transfer.list" and "system.new.dat" to folder "baja"
  3. Now open "baja" folder and type this on terminal
  
          wget https://github.com/xpirt/sdat2img/raw/master/sdat2img.py
      
          chmod +x sdat2img.py
      
          ./sdat2img.py system.transfer.list system.new.dat system.img
      
  4. After complete you will find raw file image named "system.img"
  5. Open that file using disk image mounter which is already installed on ubuntu 14.04
  6. And voila you have acces to file inside "system.img"
