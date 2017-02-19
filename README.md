
# Get the code: 

 apt-get update -qq -y && apt-get install git
 
 git clone  https://github.com/keldnorman/masscan-util-to-images.git

INSTALL PRE REQ. FOR:
# scan-and-screenshot

apt-get install ratpoison xvfb masscan imagemaigck golang morgrify iptables
 
export GOPATH=/home/[YOUR USER]/go && go get github.com/adnanh/webscrot
 
Alter the WEBSCROT variable in the script to match your user directory

INSTALL PRE REQ. FOR:
# scan-and-screenshot-extra

apt-get install ratpoison xvfb masscan imagemaigck golang morgrify iptables

git clone https://github.com/yaph/webshots.git

ln -s /path/to/webshots/webshots $HOME/bin

ln -s /path/to/webshots/webshots.js $HOME/bin

Alter the WEBSHOTS variable in the script to point to your webshot location

# RUN
chmod +x ./scan-and-screenshot*
./scan-and-screenshot 10.0.0.0/24

./scan-and-screenshot 172.16.0.0/16

You can also screenshot external ip ranges..
