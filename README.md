# jupyterlab-php-bash

```bash
git clone https://github.com/jooni22/jupyterlab-php-bash.git
cd jupyter-php-bash
docker build -t jupyter-php-bash . 
docker run -d -p 8888:8888 jupyter-php-bash 
docker_last_ID=$(docker ps -n -1 | tail -n 1 | cut -d " " -f1) 
docker logs --tail 10 $docker_last_ID
```
