# Django + VueJS-2 Basic Setup

This is a boilerplate project for using vuejs-2 with Django. The project was inspired by the lack of adequate documentation on the use of Django with VueJS and hardships faced by most people while trying to integrate these two frameworks. The setup can be downloaded and used as the starter settings for any Django-VueJS projects in futur.

### Features

* Django backend in `./backend`
* Vuejs (v2) frontend in `./frontend`
* Hot-reload with vue-loader
* eslint linter integration
* Makefile to make your life easy


### Development environment setup

Ensure you have the latest versions of <a href="https://help.pythonanywhere.com/pages/Node/"> npm and node (v4 and above) </a> to esure you can run es5 scripts without errors since VueJS is based on the es5 syntax.

Foremost, be sure to create a virtual environment for your project since the default python instance available will be used. Use the mkvirtualenv command as follows:

```bash
$ mkvirtualenv nenv
```

Install MySQL client as follows:

For Python 2.7

```bash
$ pip install mysql-python
```

For Python 3.x

```bash
$ pip install mysqlclient
```

The requirements.txt file I meant to reduce the number of commands to execute.

These steps will install all required dependencies including development ones, run migrations and start dev server.

```bash
$ make dev
$ make migrate
$ make run
```

### Deployment

These steps will install productio dependencies and build vuejs application to `static/dist` folder.

```bash
$ make prod
$ make build
```


