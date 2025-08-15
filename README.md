# CNNtraining_deepPeNSiev
## 1. install
   #### docker desktop  https://www.docker.com/products/docker-desktop
   #### Git             https://git-scm.com/downloads

```bash
git clone https://github.com/RaulMurillo/deep-pensieve.git
cd deep-pensieve
```

## 2. run docker 
```bashhttps://github.com/Wuyueeeee/CNNtraining_deepPeNSiev/blob/main/README.md
docker build -t deep_pns -f Dockerfile .
docker run -it --rm -v "${PWD}:/workspace" deep_pns /bin/bash 
```

## 3. start training
```bash
cd /workspace/src/TensorFlow
python3 lenet5_train.py float32
```
