####
venv
####

Venv is a set of shell functions for managing `virtualenv
<http://pypi.python.org/pypi/virtualenv>`_ tool. It supports both bash and
zsh.

Features
========

1. All virtual environments are kept in one place
2. Support for bash and zsh
3. Single command as entry point

Setup
=====

Bash users, add following line to ~/.bashrc:

::

    source /path/to/venvinit

Zsh users, place venvinit file somewhere in your fpath and autoload it:

::

    fpath=(~/.zsh/functions $fpath)
    autoload -U venvinit && venvinit


Basic usage
===========

Create virtualenv:

::

    venv create sandbox

List all your virtual environments:

::

    venv list

Activate it:

::

    venv activate sandbox

Deactivate:

::

    venv deactivate

Remove virtual environment:

::

    venv remove sandbox
