# jupyter_my-notebook
 Data Science project template

## To start new Data Science project:

1. Copy this repo

Create a new directory, cd into it, and then run

```
git init
git pull https://github.com/glebmikha/data-science-project-template.git
```

2. Add your favorite Python modules to ./docker/jupyter/requirements.txt. For example:

```
xgboost
tensorflow==1.6.0
```

3. Start containers

```
docker-compose up
```

4. Copy a jupyter url from terminal and open it in your browser.

5. Stop containers

```
docker-compose down
```

6. Update images
```
docker-compose build --pull
```

7. Clean Docker's mess

```
docker rmi -f $(docker images -qf dangling=true)
```

Sometimes it is useful to remove all docker's data.

```
docker system prune
```