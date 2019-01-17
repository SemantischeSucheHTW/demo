# Demo

Ensure you have the following utilites setup:
- [docker](https://www.docker.com/products/docker-desktop)
- [docker compose](https://docs.docker.com/compose/install/)
- [git lfs (Large File Storage)](https://git-lfs.github.com/), make sure to have run `git lfs install` after setup.

```
git submodule init
git submodule update --recursive
sudo docker-compose up # depending on your system sudo might not be necessary
sudo docker exec -it html_extractor python3 generateparseorders.py
```
