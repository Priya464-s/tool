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

## BurpSuite Linux pre-requisites installation as root
- [Oracle java version "1.8.0_291"](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html)
- Maven
- Python 2 + 3
- Radamsa to fuzz your programs
- RVM
- Ruby
- Jython
- jRuby

Execute
```
curl -sSL https://rvm.io/mpapis.asc | gpg --import - && curl -sSL https://rvm.io/pkuczynski.asc | gpg --import - && source /usr/local/rvm/scripts/rvm && \curl -sSL https://get.rvm.io | bash -s stable --rails && rvm install jruby && apt install jython libcanberra-gtk-module libcanberra-gtk3-module gcc make git wget -y && pip install frida && python3 -m pip install frida && pip install Pyro4 && python3 -m pip install Pyro4 && cd /usr/share && git clone https://gitlab.com/akihe/radamsa.git && cd radamsa && make && make install && echo "HAL 9000" | radamsa && cd && cd /usr/share && git clone https://github.com/PortSwigger/software-vulnerability-scanner.git && apt install maven -y && cd software-vulnerability-scanner && mvn package && cd
```

    
# BurpSuite Community v2022.9.6
[Click to download](https://portswigger-cdn.net/burp/releases/download?product=community&version=2022.9.6&type=Linux) and install it executing:
    
    chmod +x burpsuite_community_linux_v2022_9_6.sh && ./burpsuite_community_linux_v2022_9_6.sh
    
# BurpSuite Pro v2022.9.6
[Click to download](https://portswigger-cdn.net/burp/releases/download?product=pro&version=2022.9.6&type=Linux) and install it executing:
    
    chmod +x burpsuite_pro_linux_v2022_9_6.sh && ./burpsuite_pro_linux_v2022_9_6.sh
    
# Install extensions in BurpSuite Community

Open Burp Suite -> Extender -> Options -> Python Enviroment -> Location of jython standalone JAR file:

/usr/share/jython/bin/jython
#
Open Burp Suite -> Extender -> Options -> Ruby Enviroment -> Location of jRuby JAR file:

/usr/local/rvm/rubies/jruby-9.2.9.0/lib/jruby.jar
#
Open Burp Suite -> Extender -> BApp Store -> Sort by Last updated-> Install all extensions
#
Open Burp Suite -> Extender -> Extensions -> Add -> Extension file (.jar) Select file -> burp-vulners-scanner-1.2.jar

You cand find it in this folder /usr/share/software-vulnerability-scanner/target

#
Now login/singup [here](https://vulners.com/userinfo) and generate/copy your API Key

Is time to open BurpSuite TAB called Software Vulnerability Scanner and add yours.

# BurpSuite Pro Linux v2022.2.4
#
Manual activation
#
  java -jar keygen.jar
#
Location

  cd ~/Downloads/Burp-Suite
#
open keygen(activator) 👇🏼

    java --illegal-access=permit -Dfile.encoding=utf-8 -javaagent:/home/%username%/Downloads/Burp-Suite/loader.jar -noverify -jar /home/%username%/Downloads/Burp-Suite/burpsuite_pro_v2021.12.1.jar
    
#
# Install extensions in BurpSuite Pro

Open Burp Suite -> Extender -> Options -> Python Enviroment -> Location of jython standalone JAR file:

/usr/share/jython/bin/jython
#
Open Burp Suite -> Extender -> Options -> Ruby Enviroment -> Location of jRuby JAR file:

/usr/share/jruby/bin/jruby
#
Open Burp Suite -> Extender -> BApp Store -> Sort by Details-> Install all Pro extensions

#
Now login/singup [here](https://vulners.com/userinfo) and generate/copy your API Key

Is time to open BurpSuite TAB called Software Vulnerability Scanner and add yours.
