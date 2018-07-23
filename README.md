

#EC2-C5-2XL ONLY

#!/bin/bash
apt-get upgrade -y 
apt-get update -y
apt-get install -y libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev git
git clone http://github.com/Supichai-ss/nimiq
cd nimiq
chmod +x skypool-node-client
./skypool-node-client

#EC2-C5-4XL ONLY

#!/bin/bash
apt-get upgrade -y 
apt-get update -y
apt-get install -y libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev git
git clone http://github.com/Supichai-ss/nimiq
cd nimiq
chmod +x skypool-node-client
mv config-16.txt config.txt
./skypool-node-client
