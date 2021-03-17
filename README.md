# Reactのチュートリアルをやった

Reactの環境をDockerを使用して構築し，[Reactのチュートリアル](https://ja.reactjs.org/tutorial/tutorial.html#setup-option-2-local-development-environment)を行った

## 環境構築の手順

dockerとdocker-composeはインストール済みのものとして進める


1. Dockerfileをおいてあるディレクトリで, サービスをビルドする 

```
$ docker-compose build
```

2. create-react-appとReactのインストール

```
$ docker-compose run --rm node sh -c "npm install -g create-react-app && create-react-app react-sample"
```

3.  コンテナの起動とReactの実行

- コンテナ起動

```
$ docker-compose up
```


- 最新のイメージを使ったコンテナを起動する

```
$ docker-compose up --build
```