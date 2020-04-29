#!/bin/bash

clear

black="\033[0;30m"
darkgray="\033[1;30m"
lightgray="\033[0;37m"
red="\033[0;31m"
lightred="\033[1;31m"
green="\033[0;32m"
lightgreen="\033[1;32m"
orange="\033[0;33m"
yellow="\033[1;33m"
blue="\033[0;34m"
lightblue="\033[1;34m"
purple="\033[0;35m"
lightpurple="\033[1;35m"
cyan="\033[0;36m"
lightcyan="\033[1;36m"
white="\033[1;37m"


echo -e $lightred"██╗   ██╗ ██████╗ ██╗   ██╗████████╗██╗   ██╗██████╗ ███████╗    ██████╗ ██╗     "
echo -e $lightred"╚██╗ ██╔╝██╔═══██╗██║   ██║╚══██╔══╝██║   ██║██╔══██╗██╔════╝    ██╔══██╗██║     "
echo -e $lightred" ╚████╔╝ ██║   ██║██║   ██║   ██║   ██║   ██║██████╔╝█████╗█████╗██║  ██║██║     "
echo -e $lightred"  ╚██╔╝  ██║   ██║██║   ██║   ██║   ██║   ██║██╔══██╗██╔══╝╚════╝██║  ██║██║     "
echo -e $lightred"   ██║   ╚██████╔╝╚██████╔╝   ██║   ╚██████╔╝██████╔╝███████╗    ██████╔╝███████╗"
echo -e $lightred"   ╚═╝    ╚═════╝  ╚═════╝    ╚═╝    ╚═════╝ ╚═════╝ ╚══════╝    ╚═════╝ ╚══════╝"
echo -e $darkgray"●●●●●●●●●●●●●●●●●●●●●●●●●●●●●●●●●●●●◥◣◥◣【$white by r3dnbl4ck ♫ $darkgray 】◥◣◥◣●●●●●●●●●●●●●●●●"

echo -e $lightred""
read -p "╚-● Enter link ➤ " varname


youtube-dl -q --extract-audio --no-playlist --audio-format mp3 $varname

spinner() {
    local i sp n
    sp='/-\|'
    n=${#sp}
    printf ' '
    while sleep 0.1; do
        printf "%s\b" "${sp:i++%n:1}"
    done
}

echo -e $white "Music Downloaded $lightgreen【✔ 】$white , restarting "
spinner &

sleep 3

kill "$!" # kill the spinner

./youtube-dl
