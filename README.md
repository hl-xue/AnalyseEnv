# DevEnv

## Scanpy-Pegasus
Build command
```bash
docker build -t xuehl/scanpy-pegasus:trisomy -f scanpy-pegasus.docker --platform linux/amd64 --no-cache .
```

[Image on Docker Hub](https://hub.docker.com/repository/docker/xuehl/scanpy-pegasus/general)

## Seurat-Signac
Build command
```bash
docker build -t xuehl/seurat-signac:trisomy -f seurat-signac.docker --platform linux/amd64 --no-cache .
```

[Image on Docker Hub](https://hub.docker.com/repository/docker/xuehl/seurat-signac/general)

## Scarf
Build image
```bash
docker build -t xuehl/scarf:trisomy -f scarf.docker --platform linux/amd64 --no-cache .
```

Run container
```bash
docker run -it -p 8888:8888 -v $PWD:/analysis xuehl/scarf:trisomy bash
```

Launch jupyter lab
```bash
cd analysis/
jupyter lab --ip 0.0.0.0 --port 8888 --no-browser --allow-root
```

[Image on Docker Hub](https://hub.docker.com/repository/docker/xuehl/scarf/general)
