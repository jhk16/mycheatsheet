# My cheat sheet


* Find string and substitute
``` bash
grep "origin" * -rl | xargs sed -i 's/origin/substitute/g'
```

* Change python specific version (3.8.0)
``` bash
# Install python packages
apt install python3.8 python3.8-dev python-pip python3-pip

# Install python3.8 to system
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.8 0

# Set primary python version when running python
sudo update-alternatives --config python

# Set primary python3 version when running python3
sudo update-alternatives --config python3

# Install packages you need
python -m pip install -U matplotlib
python -m pip install -U pandas
python -m pip install -U seaborn
```
