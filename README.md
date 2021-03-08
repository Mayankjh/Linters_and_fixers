# Linters_and_fixers

It includes hooks for:
* [isort](https://github.com/PyCQA/isort)
* [Flake8](https://github.com/PyCQA/flake8)
* [Bugbear](https://github.com/PyCQA/flake8-bugbear)
* [Black](https://github.com/psf/black)
* [Mypy](https://github.com/python/mypy)
* [coverage.py](https://github.com/nedbat/coveragepy/tree/coverage-5.3)
* [Bandit](https://github.com/PyCQA/bandit)
* [Safety](https://github.com/pyupio/safety)


Steps for running the pre-commit hooks: 
1. Clone this repository: `git clone `
2. Remove Websiteblocker.py
3. Install pre-commit hooks `pre-commit install` 
4. Change some code and commit to *your own* repository (triggering the pre-commit hooks)
5. To manually trigger code `pre-commit run --all-files`
 