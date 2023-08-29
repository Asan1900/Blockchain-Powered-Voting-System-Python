# Blockchain Voting System

Welcome to my Blockchain Voting System. This project is currently under development, but you can already test some of its functionalities.

## Installation

To get started, follow these steps:

1. Clone the repository.
2. Navigate to the project directory.

Install the required Python packages using pip:

```sh
$ pip install -r requirements.txt

Running the System
Start a blockchain node server and the application using the following commands:

```
# For Windows users, follow this link: https://flask.palletsprojects.com/en/1.1.x/cli/#application-discovery
$ export FLASK_APP=service.py
$ flask run --port 8000

```sh 
# Running the System
# Start a blockchain node server and the application using the following commands:


$ python app.py

``` 
This will initiate a blockchain node instance on port 8000 and launch the application concurrently. The application should be accessible at http://localhost:5000.

Sample Scenario
Here's a sample scenario you might want to try out:

Suppose you want to register two new nodes (port 8001 and 8002) with the already running node at port 8000. You can use the following cURL requests:

Register node at port 8001:

``` 
curl -X POST \
  http://127.0.0.1:8001/register_with \
  -H 'Content-Type: application/json' \
  -d '{"node_address": "http://127.0.0.1:8000"}'

 
Register node at port 8002:
curl -X POST \
  http://127.0.0.1:8002/register_with \
  -H 'Content-Type: application/json' \
  -d '{"node_address": "http://127.0.0.1:8000"}'

```

Feel free to explore and experiment with the Blockchain Voting System!

Please note that this system is still in development, and more features and improvements will be added in the future.