# Getqd_2014 Django Project #
## Prerequisites ##

- python >= 2.5
- pip
- virtualenv/wrapper (optional)

## Installation ##
### Creating the environment ###
Create a virtual python environment for the project.
If you're not using virtualenv or virtualenvwrapper you may skip this step.

#### For virtualenvwrapper ####
```bash
mkvirtualenv --no-site-packages getqd_2014-env
```

#### For virtualenv ####
```bash
virtualenv --no-site-packages getqd_2014-env
cd getqd_2014-env
source bin/activate
```

### Clone the code ###
Obtain the url to your git repository.

```bash
git clone https://github.com/getqd/getqd_2014.git getqd_2014
```

### Install requirements ###
```bash
cd getqd_2014
pip install -r requirements.txt
```

### Configure project ###
```bash
cp conf/__local_settings.py local_settings.py
vi getqd_2014/local_settings.py
```

### Sync database ###
```bash
python manage.py syncdb
python manage.py migrate
```

## Running ##
```bash
python manage.py runserver
```

Open browser to http://127.0.0.1:8000
