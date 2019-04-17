# Contributor Guide

The contributor guide has the following sections:

- [Setup](#setup)
- [Test](#test)

## Setup

To get your development environment setup, you first must clone the source repository:

```
git clone git@github.com:NLPKit/SubjectMatter.git
```

To build and test the code, it is required to have the following minimal toolset installed:

- [Python (3.7)](https://www.python.org/downloads/)

Install the Python dependencies with `pip`:

```bash
pip install -r requirements.txt
```

## Test

From the root of the repository, you can run the following to run all of the tests:

```bash
python -m unittest discover test
```

### Running A Full CI Build Locally

The CircleCI configuration includes a number of lint and test steps. If you'd like to run a complete, representative CI build locally, download the `circleci` CLI tool. See the [official installation instructions](https://circleci.com/docs/2.0/local-cli/#installing-the-circleci-local-cli-on-macos-and-linux-distros) for download information.

Once you have the tool installed in your path, run the following from the root of the repository:

```bash
circleci build
```
