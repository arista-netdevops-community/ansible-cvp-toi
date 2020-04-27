# TOI Lab preparation using Python Virtual Environment.

All the labs have been built using Arista Test Drive topology. Start an ATD or ask to your Arista representative to access to a lab.

To run labs, you can use either a docker container pre-configured or configure your system with Python and virtualenv.

## Install Virtual environment.

> For people already running virtual env

Run TOI in a python's virtual environment:

```shell
# Clone repository
git clone https://github.com/titom73/ansible-cvp-toi.git

# Move to directory
cd ansible-cvp-toi
```

### Install Python virtual Environment

> Other venv setup might be used as well.

```shell
# Install virtualenv if not part of your system
$ python -m pip install virtualenv

# Create a virtual env named .venv
$ virtualenv --no-site-packages -p $(which python3) .venv

# Activate virtualenv
$ source .venv/bin/activate
```

### Install Requirements

```shell
$ pip install -r requirements.txt
```

### Configure CloudVision IP Address

Go to [`labs`](../labs/) folder and do the following command:

```shell
$ cd labs

# Edit inventory file
$ vim inventory.yml
```
