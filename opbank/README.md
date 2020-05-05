# OP Bank API Sandbox

[![Chat on Gitter](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/meeshkan/community)

<!-- TODO: Add link to Meeshkan blog once published -->
This repository contains the source code for our article: [How to create a sandbox for the OP Bank API]().

## What's in this document

* [Getting started](#getting-started)
    * [Setting up the repository](#setting-up-the-repository)
    * [Installing HMT](#installing-hmt)
    * [Starting the mock server](#starting-the-mock-server)
    * [Running the tests](#running-the-tests)
* [Mentioned resources](#mentioned-resources)
* [Contributing](#contributing)
* [Tell us what you think](#tell-us-what-you-think)

## Getting started

⚠️**Prerequisites**:
- [Python 3.6+](https://www.python.org/downloads/)

### Setting up the repository

Clone this repository and move into the directory:
```bash
git clone https://github.com/meeshkan/hmt-examples.git
cd hmt-examples
```

Once you're there, [create a virtual environment](https://docs.python.org/3/tutorial/venv.html). 

Then, install the dependencies:
```bash
pip install -r requirements.txt
```

Finally, move into the `opbank` directory:
```bash
cd opbank
```

### Installing HMT

The HTTP Mocking Toolkit (HMT) is written in Python and available as a [PyPi package](https://pypi.org/project/hmt/). 

To install HMT via [pip](https://pip.pypa.io/en/stable/installing/), run:
```bash
pip install hmt
```

To make sure it's installed properly, run:
```bash
hmt --help
```

### Starting the mock server

Once HMT is installed, run the following command to spin up your mock OP Bank server:
```bash
hmt mock ./spec/openapi.yml
```

### Running the tests

You can run the tests with [`pytest`](https://docs.pytest.org/en/latest/):
```bash
pytest
```

## Mentioned resources

Here are a few of the resources mentioned in our tutorial:
- 📖 [OP Bank API Documentation](https://op-developer.fi/docs)
- 🔨 [`http-types`](https://github.com/Meeshkan/http-types/)
- ️🔗 [Kong Gateway](https://konghq.com/kong/) 

## Contributing

Notice a bug? Have any questions? The best way to get involved is to [open an issue](https://github.com/meeshkan/hmt-examples/issues).

Please note that this project is governed by the [Meeshkan Community Code of Conduct](https://github.com/meeshkan/code-of-conduct). By participating, you agree to abide by its terms.

## Tell us what you think

At [Meeshkan](https://meeshkan.com/), we're working to improve how people test their products. So no matter if you loved or loathed our tutorial, we want to hear from you. 

Here are some ways you can get in touch:
- [Open an issue](https://github.com/meeshkan/hmt-examples/issues)
- [Tweet at us](https://twitter.com/meeshkanml)
- [Reach out on Gitter](https://gitter.im/Meeshkan/community)