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
使用下列指令來執行建好的 container image
用 rm 是表示當 container 執行完後自動刪除
```
docker run --rm songchiu/2025cloud:container-a
docker run --rm songchiu/2025cloud:container-b
```

## Tag 命名邏輯
`<DOCKER_USERNAME>/2025cloud:<tag>`
![image](https://github.com/user-attachments/assets/6cd2af7c-8338-4edd-a9d3-d7105069e01b)
