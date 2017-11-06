# Deep Learning @ University of Helsinki 2017

This repository contains the exercises for the [Deep learning course](https://courses.helsinki.fi/en/data20001/119209014) held at the University of Helsinki in 2017.

The exercises as Jupyter notebooks that contain the problem setting and some Python code to get you started.  Solving the exercise problems require you to write some code of your own based on what you have learned in the course so far.

The recommended way to do the exercises is to use the Notebooks service at [CSC - IT Center for Science](https://www.csc.fi/).  You can also run the exercises on your own computer, or in one of the computer classes.  Below are instructions for both scenarios.


## Exercise instructions for CSC

Open https://notebooks.csc.fi/ in a web browser.  Click Haka-login and select University of Helsinki and log in using your normal university
username and password.

The first time you need to join the course group: go to the Account tab, click "Join Group" and enter the joining code
"deeplearning2017-mvzdk".

To access the exercises go to the Dashboard tab and launch a new instance of "Deep Learning Exercises 2017".  This starts a virtual machine
for you that will run for a maximum of 3 hours.  (Remember to save your results locally before that!)  Once the machine is up and running
you can click "Open in browser" to access it.  After that a file view should open up where you can access all the available exercises.

To save a local copy of your notebook click File -> Download as -> Notebook (.ipynb).  The resulting file can be uploaded to a new virtual
machine instance at CSC if you want to continue some other day (note: nothing in saved at CSC!).  This file is also what you will submit in
Moodle as your exercise solution.


## Exercise instructions for running on your own computer

If you for some reason can't or don't want to use CSC, you can also do the exercises on your own machine, or in one of the computer classes.
First you have to install all the dependencies: Jupyter, Keras and Tensorflow.  On Unix-based systems the easisest way is probably by using
virtualenv:

    virtualenv --system-site-packages -p /usr/bin/python3 env
    source env/bin/activate

    pip install --upgrade pip
    pip install --upgrade ipython
    pip install tensorflow
    pip install jupyter keras

If the above command doesn't work, try replacing pip with pip3.5.  Your system of course needs to have python and virtualenv installed
beforehand.

Next time you want to run it, you just need to enter the virtual environment you set up before:

    source env/bin/activate

Next you will need to download the notebook files for the exercises.  These can be found in the course's GitHub repository:
<https://github.com/HY-TKTL/deep-learning-course-2017>.  In the same directory where you have downloaded these, you can now run:

    jupyter notebook

This should launch the jupyter notebook viewer in your web browser.  From here on it should work as on CSC, except that the files are saved
directly to your own computer.
