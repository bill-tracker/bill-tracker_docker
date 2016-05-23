# Bill Tracker

## Table of Contents

* [Top Priority Issues](#top-priority-issues)
* [Getting Started](#getting-started)
* [Learning Resources](#learning)
* [Team Members - 2015](#team-members-2015)
* [Acknowledgements](#acknowledgements)

## <a name="top-priority-issues"></a>Top Priority Issues
Our issues that need addressing page is here https://github.com/bill-tracker/bill-tracker/issues
From that list, high priority tickets are
- search https://github.com/bill-tracker/bill-tracker/issues/150
- rap genious style annotations https://github.com/bill-tracker/bill-tracker/issues/263
- mobile https://github.com/bill-tracker/bill-tracker/issues/261
- user registration https://github.com/bill-tracker/bill-tracker/issues/155

If you have any questions about anything or need help getting started, you'll probably want to join our slack channel at https://billtracker.slack.com/  You'll need an invite from Dee for that.  You can email me at mcdermottsolutions@gmail.com and I can ask Dee to send you the slack invite.  Sorry about the runaround, we're super excited that you're interested and would really love some new blood in this project!

## <a name="getting-started"></a>Getting Started on your Local Computer<br />Using our Texas 4-Step Process<sup>TM</sup>:

**1. Install Docker Compose:**

https://docs.docker.com/compose/install/

**2. Instal Git:**

https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

**3. Clone our repo:**

    git clone https://github.com/bill-tracker/bill-tracker_docker.git ./bill-tracker && cd bill-tracker

**4. Run server (give it some time on the first time):**

    docker-compose up

**Check out this app on your browser:**

Go to: http://localhost:8000/

**Django shell** (Optional, good for checking the contents of the models during development or testing, or just generally trying things out):

    docker-compose run web python manage.py shell

## <a name="learning"></a>Learning Resources

**JavaScript**

* [Codecademy - JavaScript](https://www.codecademy.com/learn/javascript)
* [Codecademy - jQuery](https://www.codecademy.com/learn/jquery)
* [Free Code Camp](https://www.freecodecamp.com/)

**Python**

* [Codecademy - Python](https://www.codecademy.com/learn/python)
* [Learn Python the Hard Way](http://learnpythonthehardway.org/book/)
* [Google's Python Class](https://developers.google.com/edu/python/)

**Django**

* [PyLadiesATX's Intro to Django workshop](https://github.com/sarasafavi/introdjango)

**Git**

* [Try Git](https://try.github.io/)
* [git - the simple guide](http://rogerdudler.github.io/git-guide/)
* [Git Real](https://www.codeschool.com/courses/git-real)
* [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/)
* [Pro Git, 2nd Edition (2014)](https://git-scm.com/book/en/v2)

## <a name="team-members-2015"></a>2015 Team Members

* Deepti Boddapati [@deeptiboddapati](https://github.com/deeptiboddapati)
* Filip Drozdowski [@fdrozdowski](https://github.com/fdrozdowski)
* Ed Solis [@edsfocci](https://github.com/edsfocci)
* Mark McDermott [@mcdermottsolutions](https://github.com/mcdermottsolutions)
* Logan Robinson [@loganrobinson](https://www.linkedin.com/in/loganrobinson)
* Nick Kasten [@kastentx](https://github.com/kastentx)
* Laura Arthur [@Lautte](https://github.com/Lautte)
* Rahul Putha [@rahulputha](https://github.com/rahulputha)

## <a name="acknowledgements"></a>Acknowledgements

Our Texas 4-Step Process<sup>TM</sup> and this Docker container was made
possible by the
[Docker Compose and Django Quickstart Guide](https://docs.docker.com/compose/django/).
(Thank the contributors that you don't need to install and configure Python and 
PostgreSQL on your machine, among other things)

## <a name="getting-started-no-docker"></a>Getting Started on your Local Computer<br />Without Docker

**Install Python 3:**

https://www.python.org/downloads/ or

http://conda.pydata.org/miniconda.html

Note: The core team will develop this project in Python 3, so it is recommended 
that you do the same.

**Instal Git:**

https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

**Clone our repo:**

    git clone https://github.com/bill-tracker/bill-tracker_docker.git ./bill-tracker && cd bill-tracker

**Install PostgreSQL:**

http://www.postgresql.org/download/

**Install Psycopg:**

http://initd.org/psycopg/docs/install.html

**Install all *local* dependencies:**

    pip install -r requirements.txt

or (needs verification):

https://groups.google.com/a/continuum.io/forum/#!topic/conda/PiM9sjWyXFU

    conda create -n new environment --file requirements_local.txt

Or, you can install the dependencies manually if you wish / need.

**Initialization:**

    python manage.py migrate

**Run server:**

    python manage.py runserver

**Check out this app on your browser:**

Go to: http://localhost:8000/

**Django shell** (Optional, good for checking the contents of the models during development or testing, or just generally trying things out):

    python manage.py shell

**Alternative method if the above doesn't work for you**

```
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver

python3 manage.py flush
```
