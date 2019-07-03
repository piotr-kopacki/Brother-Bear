<h1 align="center">Brother-Bear</h1>
<p align="center">My solution to JMR Junior Python Develeper recruitment task.</p>


## Installation

Requires [Python](https://www.python.org/) 3.5+ to run.

Install the dependencies, apply migrations, and start the server.

```sh
$ cd .\Brother-Bear\
$ pip install -r requirements.txt
$ python3 manage.py makemigrations
$ python3 manage.py migrate
$ python3 manage.py runserver
```

## Running with docker

 ```sh
$ cd .\Brother-Bear\
$ docker build -t bear .
$ docker run -p 8000:8000 -i -t bear
```


## Running the tests

```sh
$ python3 manage.py test
```

## API Endpoints

`/` - ( POST | GET ) Create shortened url  
`/<str:id>` - ( GET ) Returns shortened url
