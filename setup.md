# setup git
git config --global user.name "name"
git config --global user.email "name@host.com"

# setup Janus vim distribution
curl -L https://bit.ly/janus-bootstrap | bash

# setup python environments and alias them
mkdir ~/pyEnvs

python3 -m venv --python=/usr/bin/python2.6 ~/pyEnvs/kernel2.6
python3 -m venv --python=/usr/bin/python3.5 ~/pyEnvs/kernel3.5

alias py2='source ~/pyEnvs/kernel2.6/bin/activate'
alias py3='source ~/pyEnvs/kernel3.5/bin/activate'

# using py3, get glances:
py3
pip install --upgrade pip
pip install glances

