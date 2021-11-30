<img src="https://www.howtogeek.com/wp-content/uploads/2012/02/wine-header.png?height=200p&trim=2,2,2,2" width="50%" >

# WHAT IS WINE ?
  Wine (originally an acronym for "Wine Is Not an Emulator") is a compatibility layer capable of running Windows applications on several POSIX-compliant operating  systems, such as Linux, macOS, & BSD. Instead of simulating internal Windows logic like a virtual machine or emulator, Wine translates Windows API calls into POSIX calls on-the-fly, eliminating the performance and memory penalties of other methods and allowing you to cleanly integrate Windows applications into your desktop.

## INSTALLATION
  If your system is 64 bit, enable 32 bit architecture (if you haven't already):
   
    sudo dpkg --add-architecture i386 

Download and add the repository key:

    wget -nc https://dl.winehq.org/wine-builds/winehq.key
    sudo apt-key add winehq.key
    
Add the repository:

For this version:	Use this command:
Ubuntu 21.10	

    sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ impish main'
Ubuntu 21.04	

    sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ hirsute main'
Ubuntu 20.10	
  
    sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ groovy main'
Ubuntu 20.04 and Linux Mint 20.x

    sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ focal main'
Ubuntu 18.04 and Linux Mint 19.x

    sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ bionic main'
    
Update packages:

    sudo apt update
Then install one of the following packages:

Stable branch	
      
     sudo apt install --install-recommends winehq-stable
Development branch	
    
    sudo apt install --install-recommends winehq-devel
Staging branch	

    sudo apt install --install-recommends winehq-staging
    
    
    
    
