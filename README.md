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
The last command will kick off the parsing, extracting and indexing pipeline.
This will take a while to finish.

The following services are exposed to the host:
- `mongo-express` on port 9090.
- `frontend` on port 8080.
- `rest-search` servicing the frontend on port 8181.
- `spellchecker` servicing the frontend on port 8282.
