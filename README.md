# Linters_and_fixers

It includes hooks for:
* [isort](https://github.com/PyCQA/isort) - It sorts your import statements
* [Flake8](https://github.com/PyCQA/flake8) - Flake8 is a wrapper around pyflakes, pycodestyle and Ned Batchelder’s McCabe script essentially checking for conformance to the PEP 8 code style standard.If any non-conformances are detected the tool will output a warning with an error code.
* [Bugbear](https://github.com/PyCQA/flake8-bugbear) - Bugbear is a plugin for flake8 containing some rules for errors and warnings that do not fit within pyflakes or pycodestyle. An example of this is rule B009 eg: Do not call getattr(x, 'attr'), instead use normal property access: x.attr. Missing a default to getattr will cause an AttributeError to be raised for non-existent properties. There is no additional safety in using getattr if you know the attribute name ahead of time.
* [Black](https://github.com/psf/black) : Black is an (awesome) opinionated code formatter adhering to PEP8 (as much as possible).
* [Mypy](https://github.com/python/mypy) : Using Mypy you can add type hints (PEP 484) to your code and check your code for type errors.
* [coverage.py](https://github.com/nedbat/coveragepy/tree/coverage-5.3) :Using coverage.py you can measure the % of code executed, for example when running pytest. These metrics give you an indication how much of your code is covered by software tests. Of course, the coverage percentage does not indicate the quality of software testing.
* [Bandit](https://github.com/PyCQA/bandit): Running Bandit on your code enables you to identify known security issues (e.g. the use of assert statements as checks which are removed when compiling to byte code). 
* [Safety](https://github.com/pyupio/safety): It scans your installed dependencies for known security vulnerabilities. By default it uses the safety-db database with known vulnerabilities.


Steps for running the pre-commit hooks: 
1. Clone this repository: `git clone `
2. Remove Websiteblocker.py
3. Install pre-commit hooks `pre-commit install` 
4. Change some code and commit to *your own* repository (triggering the pre-commit hooks)
5. To manually trigger code `pre-commit run --all-files`
 
