# dockerfile sample go echo with air
## 概要
- Go言語の echo の Docker ファイルのサンプルです  
- air (ホットリロード) も入れてます
- 用途  
  - echo をちょっと試したいとき  
  - echo を勉強したくて、Docker コマンドも使ってみたいとき  
## 利用方法の例
- 2024年11月13日、以下は Mac と WSL で確認しました  
- Github からダウンロードしたら、、  
  ```
  # ダウンロードして配置したディレクトリへ
  cd dockerfile-sample-go-echo-with-air

  # Docker ビルド
  docker compose build
  
  # 必要なものをインストール
  docker compose run --rm go-echo-with-air  go mod tidy

  # コンテナを起動
  docker compose up

  ※Webブラウザで http://localhost:8080/ にアクセス
  ```

