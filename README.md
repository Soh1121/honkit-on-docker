# honkit-on-docker

## 概要

Docker上で動作するHonkitのテンプレート

## 使い方

### 起動方法

```shell
$ docker compose build --no-cache
$ docker compose exec honkit bash
/app# npm run init
/app# npm run serve
```

### 接続方法

http://localhost:4000
