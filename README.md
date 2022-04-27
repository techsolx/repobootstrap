# Name of Project

This is a sample I use for [README.md](README.md) files,
     and for getting started on most other projects.

## Getting Started

cd into the new repo and pull the files in individually like this:
```bash
curl -O https://raw.githubusercontent.com/techsolx/repobootstrap/main/README.md & \
curl -O https://raw.githubusercontent.com/techsolx/repobootstrap/main/LICENSE & \
curl -O https://raw.githubusercontent.com/techsolx/repobootstrap/main/.editorconfig & \
curl -O https://raw.githubusercontent.com/techsolx/repobootstrap/main/.pre-commit-config.yaml & \
curl -o .gitignore https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore
```

Something like this could also work:
```bash
export PROJECT=NewProjectName
```
then do:
```bash
git clone --depth=1 --quiet --branch=main git@github.com:techsolx/repobootstrap.git $PROJECT && \
cd ./$PROJECT && \
rm -rf ./.git && \
git init && \
curl -o .gitignore https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore && \
unset PROJECT

```

### Assumptions:
* What you need to make it go
* A second bullet

### The Makefile

All management is via the Makefile, this is to make the project easy to
transition to ci/cd tooling.

### Description

The above make command will create it will also update...

### Prerequisites

Access to an aws account, docker and packer, etc...

### Installing

Fork then clone the repo, run the make file

```bash
make example
```

## Running the tests

Run tests to ensure that required is installed.

## Versioning

The more I look the more I am a fan of semver...

## Authors

* **John MacTavish** - *Initial work* -
[TechSolX](https://github.com/techsolx)

See also the list of
[contributors](<project>/<repo>/graphs/master)
who participated in this project.

## License

This project is licensed under the MIT License - see the
[LICENSE](LICENSE) file for details

## Acknowledgments

* Stack Overflow for all the other stuff I can't remember.
