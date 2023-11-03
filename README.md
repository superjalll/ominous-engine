
#!/bin/bash

echo -e "\033[0;35m"
echo "┘┘┘ ̶ ̶S̶u̶p̶e̶r̶j̶a̶l̶l̶l̶";
echo -e "\e[0m"

sleep 2

# set vars
AVAIL_PORT=30333
if [ ! $NODENAME ]; then
	read -p "Enter node name: " NODENAME
	echo 'export NODENAME='$NODENAME >> $HOME/.bash_profile
fi
source $HOME/.bash_profile
echo "export AVAIL_PORT=${AVAIL_PORT}" >> $HOME/.bash_profile
echo '================================================='
echo -e "Your node name: \e[1m\e[32m$NODENAME\e[0m"
echo -e "Your port: \e[1m\e[32m$AVAIL_PORT\e[0m"
echo '================================================='
sleep 2

echo -e "\e[1m\e[32m1. Updating packages... \e[0m" && sleep 1
