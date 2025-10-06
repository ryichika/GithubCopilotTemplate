# プロジェクト構造
このドキュメントは、BookManagementWeb（ASP.NET8.0）プロジェクトのファイル構造を説明します。

## ディレクトリ構造
```
BookManagementWeb
|---- .github//architecture/    # 開発ルールに関するmdファイルを配置するフォルダ
|  |---- codingrule.md          # コーディングルール
|  |---- dictionary.md          # 用語リスト
|  |---- product.md             # 製品概要
|  |---- structure.md           # プロジェクト構造
|  |---- techstack.md           # 技術スタック
|---- Properties/               # プロジェクト設定
|  |---- launchSettings.json    # 起動設定
|---- wwwroot/                  # 静的ファイル（CSS、画像等）
|  |---- css/                   # cssファイルを配置するフォルダ
|  |---- js/                    # Javascriptファイルを配置するフォルダ
|  |---- lib/                   # Javascript用の外部パッケージを配置するフォルダ
|  |---- favicon.ico            # favicon（ファビコン用ファイル
|---- Pages/                    # cshtmlファイルを配置するフォルダ
|  |--- Shared/                 # 複数の画面で共通するレイアウトのcshtmlファイルを配置するフォルダ
|---- appsettings.json          # アプリケーション設定
|---- Program.cs                # アプリケーションのメインエントリポイント
|---- BookManagementWeb.csproj  # プロジェクトファイル
|---- BookManagementWeb.sln     # ソリューションファイル
|---- docs/                     # ドキュメントファイルを配置するフォルダ
|  |---- [サブシステム名]/       
|    |---- [業務名]/            
|       |---- requirement.md    # 要件定義
|       |---- design.md         # 設計
|       |---- task.md           # 作業タスク 
```

## 主要ディレクトリの説明

### `.github//architecture`
アーキテクチャ関連のドキュメント（コーディングルール、用語、製品概要、プロジェクト構造、技術スタック）に関するファイルを配置するフォルダ
### `wwwroot`
本アプリで使用するcssファイル、jsファイル、外部パッケージを配置するフォルダ
### `Pages`
本アプリで使用するcshtmlファイルを配置するフォルダ
複数のcshtmlファイルで共通するレイアウト（cshtmlファイル）は、Pages/Sharedフォルダに配置する
### `docs`
本アプリに要求される要件や基本設計に関するドキュメントを配置するフォルダ
- requirement.md: 本業務に要求される要件内容を定義
- design.md: 本業務の設計内容（ワイヤーフレーム）を定義

例: 書籍管理サブシステムの場合
```
|  |---- BookManagement/
|    |---- AddBook/     
|       |---- requirement.md
|       |---- design.md     
|       |---- task.md
```
