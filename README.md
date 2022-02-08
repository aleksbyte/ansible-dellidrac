DELL iDRAC misc.,random notes.


ansible-galaxy collection install -r requirements.yml -p ./collections/
# add omsdk
git clone https://github.com/dell/omsdk.git
cd omsdk
pip3 install wheel
pip3 install -r requirements-python3x.txt
sh build.sh 1.2 423 # Note: Numbers may change based on current version. See the OMSDK repo for current.
cd dist
pip install omsdk-1.2.423-py2.py3-none-any.whl
