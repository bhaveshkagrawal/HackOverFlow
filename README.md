## HackOverFlow: Building Communities

[![Build Status][build-image]][build-url] 
[![License](http://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)

[build-image]: https://travis-ci.org/ialbert/biostar-central.svg?branch=4.0
[build-url]: https://travis-ci.org/ialbert/biostar-central/builds

HackOverFlow is a [Python][python] and [Django][django] based Q&A software.
It is a simple, generic, flexible and extensible Q&A framework.

The site has been developed by Bidgely employees for internal and client usage. It aims
to address the requirements and needs that people have.

The software is open source and free to use under the MIT License.

### Features

* Q&A: questions, answers, comments, user moderation, voting, reputation, badges, threaded discussions
* RSS Planet: feed aggregation from different sources
* External authentication: authenticate users with a different web service
* Email integration: import previous posts from mailing lists 
* Low resource utilization and easy deployment. 

Requirements: `Python 2.7`

### Documentation

The documentation:

* [Install](docs/install.md)
* [Manage](docs/manage.md)
* [Deploy](docs/deploy.md)
* [Customize](org/bioconductor/README.md)

The source for the documentation can be found in  the [docs](./docs) folder.

### Quick Start

From the HackOverFlow source directory:

    # Install the requirements.
    pip install --upgrade -r conf/requirements/base.txt

    # Initialize database, import test data, index for searching and run the server.
    ./hackOverFlow.sh init import index run

Visit `http://www.lvh.me:8080` to see the site loaded with demo data.

The `www.lvh.me` domain resolves to `127.0.0.1` your local host 
with a proper domain name. You may just as well use `http://localhost:8080` or `http://127.0.0.1`.

In the demo site the user emails are built from the database ids like so: `1@lvh.me`, `2@lvh.me`.
The demo user passwords are identical to the emails
and you may use these to log into your test site as any of the users.

The user with the email `1@lvh.me` has staff level permissions and
can also access the admin interface at `http://www.lvh.me:8080/admin/`.

Enjoy.
