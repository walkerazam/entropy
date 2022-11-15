# entropy
## An example of directory structure for testing

You can run the tests in the `entropy/tests` directory with:
`python -m unittest discover -s entropy`

Note that because of the simplicity of this repository, you can also run them with `python -m unittest` and it will find the unit tests.  More complex repositories will need the `discover` and `-s` search path.

A few things to note:
1. It is important to have `__init__.py` files in the package directory (not the respository root) and the `tests` directory for `unittest` to discover your tests.
2. In the `tests_entropy.py` file, do not use relative imports.  The `unittest` framework will execute the tests as if they are in the root of the repository.
