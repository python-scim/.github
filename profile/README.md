<p align="center">
  <img alt="python-scim logo" src="https://raw.githubusercontent.com/python-scim/.github/refs/heads/main/python-scim.svg" height="200">
  <h1>python-scim</h1>
</p>

Python libraries and tools to build and test SCIM 2.0 applications.

Libraries:

- [scim2-server](https://scim2-server.readthedocs.io) serves the SCIM protocol over any storage, in any web framework.
- [scim2-client](https://scim2-client.readthedocs.io) sends SCIM requests from a Python application, and checks the responses.
- [scim2-models](https://scim2-models.readthedocs.io) validates and serializes the SCIM resources and messages with Pydantic.

Integrations:

- [scim2-django](https://github.com/python-scim/scim2-django) will serve a SCIM server in a Django application.
- [scim2-fastapi](https://github.com/python-scim/scim2-fastapi) will serve a SCIM server in a FastAPI application.
- [scim2-flask](https://scim2-flask.readthedocs.io) serves a SCIM server in a Flask application.
- [scim2-sqlalchemy](https://scim2-sqlalchemy.readthedocs.io) stores the SCIM resources in the tables of an application, with the SQLAlchemy ORM.

Tools:

- [scim2-tester](https://scim2-tester.readthedocs.io) checks the compliance of a SCIM server with the RFCs.
- [scim2-cli](https://scim2-cli.readthedocs.io) queries a SCIM server from the command line.
- [pytest-scim2-server](https://github.com/pytest-dev/pytest-scim2-server) runs a SCIM server in a pytest test suite, to test a SCIM client.

The projects are mostly maintained by [Yaal Coop](https://yaal.coop).
There is no precise roadmap or deadline. If you need something in the libraries, please reach us through the bug trackers.
**We are available for hire** to help you build or integrate SCIM in your applications, or in your services ecosystem.
