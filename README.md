sudo add-apt-repository ppa:mozillateam/ppa

sudo apt update

echo '
Package: *
Pin: release o=LP-PPA-mozillateam
Pin-Priority: 1001
' | sudo tee /etc/apt/preferences.d/mozilla-firefox


sudo apt install firefox
