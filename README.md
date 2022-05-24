# Scansnap firmware

The following is a quick and dirty way to get my Scansnap S1300i working on Debian and Ubuntu.

# Installation on Debian

1. Download firmware:
        git clone https://github.com/sohnemann/scansnap-firmware.git
        
2. Run the following commands in a Terminal

        sudo mkdir -p /usr/share/sane/epjitsu
        sudo cp ./scansnap-firmware/* /usr/share/sane/epjitsu/.
        sudo cpan upgrade sane
        sudo apt-get install libsane-dev
        
3. Logout, and then re-login. 
4. Try ```sudo scanimage -L```
