# Jupyter Interview

## Setup

1. Build a new Docker image
```bash
docker build . -t jupyter-interview -f Dockerfile --platform=linux/amd64
```
2. Run the Jupyter container
```bash
docker run -it --rm -p 10000:8888 -v "${PWD}":/code jupyter-interview
```
1. Browse to [http://127.0.0.1:10000/lab](http://127.0.0.1:10000/lab)