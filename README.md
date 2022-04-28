# kubernetes-demo

此為 k8s 測試檔案，由 Node.js 轉寫，當訪問 3000 Port 時，會顯示一隻可愛的小柴犬 ><

1. 因為此程式有使用 Express 框架，所以在開始前請先至該專案資料夾內下載套件檔案：

```sh
npm install
```

<br>

2. 使用 docker build 來打包成映像檔：

```sh
docker build -t kubernetes-demo .
```

<br>

3. 使用 docker run 來啟動容器：

```sh
docker run -d -p 3000:3000 --name="kubernetes-demo" kubernetes-demo
```
<br>

4. 當我們訪問 3000 Port 就可以看到可愛的柴犬拉！(此圖片使用程式產生)

<br>

![圖片](https://raw.githubusercontent.com/880831ian/kubernetes-demo/master/images/Shiba-Inu.png)

* 此程式也有包好放在 [dockerhub](https://hub.docker.com/repository/docker/880831ian/kubernetes-demo)，需要直接測試的可以直接拉下來使用～
