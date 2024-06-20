# hello-world-project-template-python

This is the Hello World project which has all the basic files explained in our [Hello World Tutorial](https://learn.temporal.io/getting_started/python/hello_world_in_python/).

## Instructions

Ensure you have Python 3.7 or later installed locally, and access to a Temporal Cluster for development.

The fastest way to get a development cluster running on your local machine is to use [Temporal CLI](https://docs.temporal.io/cli#install).

Temporal CLI is a tool for interacting with a Temporal Cluster from the command-line interface. It includes a self-contained distribution of the Temporal Server and [Web UI](https://docs.temporal.io/web-ui) as well.

Once you've installed Temporal CLI on your platform of choice and added it to your ```PATH```, open a new Terminal window and run the following command:

```temporal server start-dev```

*  The Temporal Server will be available on ```localhost:7233```.
*  The Temporal Web UI will be available at ```http://localhost:8233```.

Next, clone this repository and switch to the cloned directory::

```bash
git clone https://github.com/temporalio/hello-world-project-template-python
cd hello-world-project-template-python
```

Create a virtual environment for your project and install the Temporal SDK:

```bash
python3 -m venv env
source env/bin/activate
python -m pip install temporalio pytest pytest-asyncio
```

Now you can run the worker and starter included in the project.

```bash
python run_worker.py
python run_workflow.py
```