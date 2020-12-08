# laravel skeleton

## 概要

Laravel でローカル開発を始めるのに必要な土台環境

## 構築される環境の構成・特色

* 構成
    * php
    * nginx
    * mysql
* 特色
    * 各種バージョンは docker-compose.yml より注入してください。
    * mysql に関しては primary & replica 両方用意されます

## 使い方

```
(local)$ cd docker
(local)$ docker-compose up -d
(local)$ docker-compose exec php bash

(docker)$ composer create-project "laravel/laravel=8.*" .
```

## 注意点

* 初回 mysql-primary が立ち上がるまでの待ち時間がテキトウです。
* そのため、初回replica関連でコケるかもしれません。

