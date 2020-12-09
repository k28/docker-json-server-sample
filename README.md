# JSONを返すAPIのモックサーバー

data/data.jsonを書き換えると、対応するJSONを返す

```
{fruits: [apple, orange]}
-> http://localhost:{port}/fruits で [apple, orange]が取得できる
```

## ファイル構成

```
├── .env            待ち受けポートの定義
├── Dockerfile
├── README.md
├── data
│   └── data.json   Mockで返すJSONを定義する
└── docker-compose.yml
```


## 使い方

```
$ docker-compose up -d
```

