# プロジェクト名

## 概要・目的

## セットアップ・インストール方法
- [setup.md](./docs/setup.md)に環境構築手順書を記載しています。

## 実行方法・使用例
- 各アプリケーションの実行方法や使用例については、[app/README.md](./app/README.md)をご参照ください。

## 構成

```bash
.
├── README.md                     # このファイル (プロジェクトの概要、目的、セットアップやインストール方法、実行方法・使用例を記載)
├── .devcontainer/...             #
│   └── devcontainer.json         #
├── .github                       # リポジトリの運用ルール・自動化などの設定
│   ├── ISSUE_TEMPLATE/           #           
│   └── PULL_REQUEST_TEMPLATE.md  #
├── .streamlit/...                # Streamlitの設定ファイル
├── .vscode                       # VSCodeの設定ファイル
├── app/                          # FastAPIやStreamlit等のアプリケーションコード
├── data/                         # 元データ、学習データ、推論データなどを格納
├── docs/                         # 各種ドキュメントを管理 (環境構築・実装方法・設計書# ) 
│   └── setup.md                  # 環境構築手順書
├── model/                        # pickleファイル等のモデル保存用
├── notebook/                     # Notebook(.ipynb)ファイルを格納 (データの可視化・一時的な分析)
├── outputs/                      # スクリプトの実行結果を格納
├── src/                          # 重要で再利用可能なコードを格納 (関数・クラス・モジュールなど) scriptsから呼び出される
├── scripts                       # 特定の目的に特化した処理を行う(モデルの学習・推論の実行・前処理など)
├── tests/                        # pytest用のテストコード
├── .env.example                  # 環境変数のサンプルや雛形を共有するためのもの
├── .gitignore                    # Gitでついせきしないファイルやディレクトリを指定 (APIキーや外部に公開したくない情報など)
├── Dockerfile                    #
├── LICENSE                       # 利用許諾条件を記載 (コードの再利用・再配布のルール、著作権の取扱)
├── compose.yaml                  #
├── uv.lock...                    # パッケージ管理のロックファイル
└── pyproject.toml                # パッケージ管理・ビルドシステムの設定
```
