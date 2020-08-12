# Setup

run clone via SSH or HTTP.

```bash
git clone git@github.com:smithstreaming/backend.git
```

create a venv directory in the same directory you cloned the backend to.
cd into the venv directory and create a virtual environment.

```bash
mkdir venv && cd venv && virtualenv backend
```

append the following variables to the activate file  ```backend/bin/activate```

```bash
export PYTHONPATH="home/{path to the directory you cloned backend to}/"
export PYTHONPACKAGES="home/{path to the directory you created venv in}/venv/backend/lib/python3.6/site-packages/"
```

activate the virtual environment

```bash
. ./venv/backend/bin/activate
```

install requirements listed in the requirements.txt file

```bash
pip install -r requirements.txt
```

run the django local server

```bash
python manage.py runserver
```
