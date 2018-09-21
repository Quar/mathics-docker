Dockerized Mathics
===========
[![](https://images.microbadger.com/badges/image/quar/mathics-docker:latest.svg)](https://microbadger.com/images/quar/mathics-docker:latest "Get your own image badge on microbadger.com")


REF https://github.com/mathics/Mathics


## Usage


#### To Start

```bash
docker run -d -p 8000:8000 --rm --name=mathics quar/mathics-docker
```

Then open browser to access `localhost:8000`


#### To Stop

```bash
docker stop mathics-docker
```

#### To Restart

```bash
docker stop mathics-docker
docker run -d -p 8000:8000 --rm --name=mathics quar/mathics-docker
```

### To Preserve Worksheet Data (when start use)

```bash
mkdir var
docker run -d -p 8000:8000 --rm --name=mathics -v $PWD/var:/root/.local/var quar/mathics-docker
```

