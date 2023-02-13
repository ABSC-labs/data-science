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
3. Browse to the URL printed at the end of the Docker container startup. You will switch the port from `8888` to `10000`.