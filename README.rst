web-presence
==============

web-presence


Installation
------------

Step 1: Create a virtualenv with pygtk
``````````````````````````````````````

--system-site-packages flag only required in linux(pygtk python package can build only with windows):

::

  virtualenv venv --system-site-packages

You can now activate the virtualenv

::

  cd venv
  source bin/activate


Step 2: Download and Instaall requiriments
``````````````````````````````````````````
download trytond and tryton from https://downloads.tryton.org/3.4/
clone nereid

::

  git clone git@github.com:openlabs/nereid.git

and install inside env with

::

  python setup.py install
  pip install -r requirements.txt

Step 3: Setup Database
``````````````````````

::

  trytond -c config.conf -d database_name --all

Step 4: Run application
```````````````````````

::

  trytond -c config.conf -d database_name
  python run_nereid.py


