Steps for making your package distributable
===========================================

*  generate the a distributable package
	1. python setup.py sdist
*  REGISTERING your package
	2. python setup.py register
*  UPLOADING your package
	3. python setup.py sdist upload

# ~/.pypirc config
    ::

        [distutils]
        index-servers =
          pypi
          pypitest

        [pypi]
        repository=https://pypi.python.org/pypi
        username=<username>
        password=<password>

        [pypitest]
        repository=https://testpypi.python.org/pypi
        username=<username>
        password=<password>