# CNNtraining_deepPeNSiev
for windows
##1. install
   docker desktop  https://www.docker.com/products/docker-desktop
   Git             https://git-scm.com/downloads

```bash
git clone https://github.com/RaulMurillo/deep-pensieve.git
cd deep-pensieve
```

##2.
```bash
docker built -t deep_pns -f Dockerfile .
docker run -it --rm -v "${PWD}:/workspace" deep_pns /bin/bash
```

##3.
```bash
python3 cifar10_train.py
```
