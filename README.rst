#####################
cookiecutter-chrisapp
#####################

A cookiecutter template for Chris plugin apps.

Quickstart
----------

The steps below show how to quickly create and setup a new Chris plugin app project.


1. Create a Python3 virtual environment for your plugin apps if you haven't created it yet::

    mkvirtualenv --python=python3 chrisapp_env


2. Install the latest Cookiecutter in ``chrisapp_env`` if you haven't installed it yet::

    workon chrisapp_env
    pip install -U cookiecutter


3. Generate a Chris plugin app project. The interactive script will ask you for the app project name::

    cookiecutter https://github.com/FNNDSC/cookiecutter-chrisapp.git


4. Create a new repository on https://github.com/FNNDSC with the same name as the app project
   directory generated by the previous cookiecutter command. Make sure that the repository is
   public. Don’t initialize the repository with a ``README``, a ``license`` or a ``.gitignore`` file.


5. Change the current working directory to the app project and initialize this local directory
   as a Git repository::

    git init


6. Add and commit the files in the local repository::

    git add .
    git commit -m "First commit"


7. Add the URL for the remote Github repository created in ``step 4`` where your local repository will be pushed::

    git remote add origin remote_Github_repository_URL (eg. https://github.com/FNNDSC/pl-neuproseg.git)
    git remote -v


8. Push the changes in your local repository to GitHub::

    git push origin master


9. Create a new automated build and repository on the ``fnndsc`` organization on https://hub.docker.com.
   Once you log in, click the Create button in the header and select Automated Build from the
   drop-down menu. The website will walk you through setting up the automated build. Next, when
   prompted for the GitHub repository that you’d like to use for the automated build select
   the repository that you just created.

10. Modify requirements.txt, Dockerfile and Python code with the proper versions of
    Python dependencies and libraries and push your changes to Github.






