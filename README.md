# CNNtraining_deepPeNSiev
## 1. install
   #### docker desktop  https://www.docker.com/products/docker-desktop
   #### Git             https://git-scm.com/downloads

```bash
git clone https://github.com/RaulMurillo/deep-pensieve.git
cd deep-pensieve
```

## 2.run docker 
```bash
docker build -t deep_pns -f Dockerfile .
docker run -it --rm -v "${PWD}:/workspace" deep_pns /bin/bash 
```
#### 如果docker run 路径有问题就把 "${PWD}:/workspace" 改成 "deep-pensieve所在文件夹地址":/workspace 

## 3.start training
#### python3 + 训练模型 + 训练目标（float32/float16/posit32/posit16/posit8）
```bash
cd /workspace/src/TensorFlow
python3 lenet5_train.py float32
```
