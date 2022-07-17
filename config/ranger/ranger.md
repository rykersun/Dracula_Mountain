ranger --copy-config=all

git clone https://github.com/dracula/pygments.git

cd pygments/

sudo mv dracula.py /usr/lib/python3/dist-packages/pygments/styles/


git clone https://github.com/alexanderjeurissen/ranger_devicons ~/.config/ranger/plugins/ranger_devicons

echo "default_linemode devicons" >> $HOME/.config/ranger/rc.conf
