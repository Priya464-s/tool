# burp-vulners-scanner

[![Current Release](https://img.shields.io/github/release/vulnersCom/burp-vulners-scanner.svg "Current Release")](https://github.com/vulnersCom/burp-vulners-scanner/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/vulnersCom/burp-vulners-scanner/total.svg "Downloads")](https://github.com/vulnersCom/burp-vulners-scanner/releases) [![PayPal](https://img.shields.io/badge/donate-PayPal-green.svg)](https://paypal.me/videns)

# Description

Burp Suite scanner plugin based on [Vulners.com](https://vulners.com) vulnerability database API
- Search fingerprints in http response (inspired by plugin "Software Version Reporter")
  and check found version in vulners.com vulnerability database
- [Experemental] Check unique URLs in vulners.com finding exploits for such paths

If Vulners Plugin detects vulnerable software it will show you CVE, advisoroies and even applicable exploits!

# How to use


[![Burp Vulners plugin Tutorial Video](https://img.youtube.com/vi/klu7PTgUrow/0.jpg)](https://vimeo.com/225078901)

## Requirements

- Burp Suite - Professional Edition
- Java 1.7
- Maven

## Installation

1. Clone repository
2. From command line run

     ```
     apt install maven -y
     ```
     ```
     mvn package
     ```
3. find burp-vulners-scanner.jar in /target folder
4. open Burp Suite -> Extender -> Add -> path to plugin.jar


## Build
Ready to install build [burp-vulners-scanner.jar](https://github.com/vulnersCom/burp-vulners-scanner/releases/latest)
#
#
#
#
# BurpSuite Linux Professional / Community 2020.1
#
    sudo apt install libcanberra-gtk-module libcanberra-gtk3-module jython jruby gcc make git wget -y
#    
    pip install frida && pip3 install frida && pip install Pyro4 && pip3 install Pyro4
    
 Please please please fuzz your programs. here is one way to get data for it:
    
    cd /usr/share && sudo git clone https://gitlab.com/akihe/radamsa.git && cd radamsa && sudo make && sudo make install && echo "HAL 9000" | radamsa && cd

#
Download from

https://portswigger.net/burp/releases/download?product=community&version=2020.1&type=Linux

And install:
    
    chmod +x burpsuite_community_linux_v2020_1.sh && ./burpsuite_community_linux_v2020_1.sh
#    
# BurpSuite Pro Linux v2.0.11beta
#
(Open BurpLoader to activate manually and offline the License - Only is neccesary do one time this step)
#
    java -jar burploader.jar
#
# Open BurpSuite (with 7GB of Memory RAM for be fastly)
#
    java -Xbootclasspath/p:burploader.jar -jar -Xmx7G burpsuite_pro_v2.0.11beta.jar
    
