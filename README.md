This is meant to be used with snapcraft parts.  
This snapcraft part allows to build programs with any version of Python.

## Usage:

To use this part, include the following in your snapcraft.yaml:

    Add "after: [python]" to your part written in python. By default, this will use the latest Python
    from the master branch to compile your program.
    If you want to specify a Python version, also add a Python part with the version as
    the source-tag value. For example, to use Python 2.7.2, use:
    parts:
        my-python-program:
        ...
        after: [python]
        python:
        source-tag: v2.7.2

