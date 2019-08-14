## Generate a new Laravel project

```bash
docker run --rm --interactive --tty \
    --volume $PWD:/app \
    --user $(id -u):$(id -g) \
    composer \
    create-project laravel/laravel --prefer-dist \
    [project_name] ["version"]
```

- Example: 
```bash
$ docker run --rm --interactive --tty --volume $PWD:/app --user $(id -u):$(id -g) composer create-project laravel/laravel --prefer-dist my_project "5.8.*"
```
___
## Generate a new Lumen project

```bash
docker run --rm --interactive --tty \
    --volume $PWD:/app \
    --user $(id -u):$(id -g) \
    composer \
    create-project laravel/lumen --prefer-dist \
    [project_name] ["version"]
```

- Example: 
```bash
$ docker run --rm --interactive --tty --volume $PWD:/app --user $(id -u):$(id -g) composer create-project laravel/lumen --prefer-dist my_project "5.8.*"
```
___
## Generate a new PHP (without framework) project

```bash
docker run --rm --interactive --tty \
    --volume $PWD:/app \
    --user $(id -u):$(id -g) \
    composer \
    init
```

- Example: 
```bash
$ docker run --rm --interactive --tty --volume $PWD:/app --user $(id -u):$(id -g) composer init
```
___