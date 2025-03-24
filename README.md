# checkmkinstall
#!/bin/bash

sudo apt update


sudo wget https://download.checkmk.com/checkmk/2.3.0p29/check-mk-raw-2.3.0p29_0.noble_amd64.deb

sudo apt install ./check-mk-raw-2.3.0p29_0.noble_amd64.deb -y

omd version

sudo omd create monitoring

sudo omd start monitoring
