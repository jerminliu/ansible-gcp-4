# Ansible Google Cloud Platform Examples

This repository contains examples of playbooks that perform various functions in Google Cloud Platform. This README will walk you through requirements for running Ansible against GCP environments and document any caveats to be aware of.

# Table Of Contents
- [Prerequisites](#prerequisites)
- [Requirements](#requirements)
- [Setup](#setup)

# Prerequisites

This document assumes you already have a linux/MacOS system with python3 and pip installed.

# Requirements

- Ansible Engine v2.6 or greater
- Python modules:
  - python >= 2.6 (Python 3 is recommended as Python 2 is now deprecated)
  - requests >= 2.18.4
  - google-auth >= 1.3.0
  - jmespath (A query language for JSON)
- A Google Cloud Platform account

# Setup

1. Create a new python3 virtual environment in which to work. Python virtual environments are generally recommended in order to mimic a full system install of Python and all of the desired modules without interfering with any system on which your application might run:

        user$ python3 -m venv /path/to/new/virtual/environment        

2. Activate your new virtual environment:

        user$ source /path/to/new/virtual/environment/bin/activate

3. Install all python modules:

        (environment) user$ pip install ansible requests google-auth jmespath
