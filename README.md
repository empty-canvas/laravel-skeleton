# laravel skelton

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
(local)$ docker-compose up -d
(local)$ docker-compose exec php bash

(docker)$ composer create-project "laravel/laravel=8.*" .
```


