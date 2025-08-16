# flask-app-template

Template with example for a Flask app (website with Python backend) that is bundled with Parcel, allowing clean use of Typescript and Sass while keeping the built website lightweight. Built and launched using Docker for simple and repeatable deployment.

## Requirements
Docker Desktop, or just Docker if you're on Linux

## Usage
1. Build the Docker image: ``docker build -t cas-interface .``
2. Run the Docker container: ``docker run -t -p 10000:10000 flask-app-template`` (Rename ``flask-app-template`` to your actual project name when copying this template)
3. Open a browser and go to 127.0.0.1:10000

Steps 1 and 2 can also be done at in one command: ``docker build -t flask-app-template . && docker run -t -p 10000:10000 flask-app-template``

## Running without Docker
This can be useful for development and debugging.

#### Requirements
1. Python
2. NodeJS

#### Setting up enviroments

1. Install all required node modules: ``npm install``
2. Python venv:
   1. Make virtual environment: ``python -m virtualenv venv``
   2. Activate the virtual environment, this is different for linux/windows
   3. Install requirements: ``pip install -r requirements.txt``

#### Building and running
1. Clean the ``dist`` folder: ``npm run clean``
2. Build: ``npm run build``
3. Run: ``npm run app``


To run the whole build/run pipeline: ``npm run start``