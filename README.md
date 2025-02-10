# fast_api_app

作成時の docker compose のバージョンは v2.31.0-desktop.2 なので、以下のコマンドで実行する。なお、永続ボリュームも作成した。

### 実行

```batch
docker compose up --build
```

### 停止

docker-compose.yml と同じディレクトリで実行。

```batch
docker compose down
```

## 仕様

サーバーが立ち上がると localhost(127.0.0.1)の 8000 番のポートで listen される。
内部では、localhost(127.0.0.1)の 8000 番のポートがコンテナの 80 番ポートに接続されており、fastapi のサーバーにリクエストが送信されるようになっている。
以下で、fastapi の仕様を確認できる。
[あなたの fastapi ドキュメント](localhost:8000/docs)
