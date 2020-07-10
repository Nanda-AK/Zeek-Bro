# Zeek-Bro



Step 1:- Install ethtool 
  sudo apt-get update
  sudo apt-get install ethtool
Check Install
  ethtool

Step 2:- #installing zeek pre-req packages
  apt-get install cmake make gcc g++ flex bison libpcap-dev libssl-dev python-dev swig zlib1g-dev

Step 3:- #get the key by running below command
  wget -nv https://download.opensuse.org/repositories/security:/zeek/xUbuntu_18.04/Release.key -O Release.key
  
  
Step 4:- #adding the key
  sudo apt-key add -< Release.key 
  

step 5:- apt-get update

#adding opensuse repos for zeek package 
sudo sh -c "echo 'deb https://download.opensuse.org/repositories/security:/zeek/xUbuntu_18.04/ /' > /etc/apt/sources.list.d/security:zeek.list"

apt-get update

apt-get install zeek-lts

press ok on pop up while installing zeek

To verify the zeek is installed go to /opt directory    

12  ls /opt/
   
13  cd /opt/zeek/bin
   
14  ./zeek -h

15  ./zeekctl -h

##Zeek is installed successfully!!
