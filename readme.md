## About

This docker container should improve generation of TYPO3 Documentation using
sphinx.

It provides the full setup and allows you to run the generation inside of
docker.

## Install

1. Clone Repository.
2. Run `docker build -t t3-sphinx .`, from within the repository.

## Run

Run `docker run -it --rm -v "$PWD":/home/t3-sphinx t3-sphinx html` from within the `Documentation` folder.

Where the last argument is the output format as provided by `_make/Makefile`.

The important part is to mount the `Documentation` folder into
`/home/t3-sphinx`. The `Documentation` folder has to contain the `_make` folder.

## Tested

Currently the following repositories / documentations were tested:

### Tutorials

- [Editors Tutorial](https://github.com/TYPO3-Documentation/TYPO3CMS-Tutorial-Editors)

### Books

- [Developing TYPO3 CMS Extensions with Extbase and Fluid](https://github.com/TYPO3-Documentation/TYPO3CMS-Book-ExtbaseFluid)
