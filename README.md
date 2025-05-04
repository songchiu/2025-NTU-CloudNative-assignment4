# 2025-NTU-CloudNative-assignment4

## Build
透過指令從兩個不同的 Dockerfile 建立兩個獨立的 container image，並各自加上 tag：
```
docker build -f Dockerfile.a -t songchiu/2025cloud:container-a .
docker build -f Dockerfile.b -t songchiu/2025cloud:container-b .
```

## 推上 docker hub
```
docker push songchiu/2025cloud:container-a
docker push songchiu/2025cloud:container-b
```

## run image
```
docker run --rm songchiu/2025cloud:container-a
docker run --rm songchiu/2025cloud:container-b
```