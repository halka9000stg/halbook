# Haruka's Self-Exposure Site

暫定セルフサイト

## 諸元

- Name: Halbook
- Publish Site: [halbook.web.app](https://halbook.web.app)
- VCS Repo(Git): [GitHub](https://github.com/halka900stg/halbook.git)
- Lang: Dart, etc.
- Kind: Dynamic, Pre-Rendering
- Service: Firebase
- Dependencies:
  - [IbisUI](https://github.com/IbisWeb/IbisUI.git)
  - [Lobiac](https://github.com/FunCobal-family/ChestDD_Language/tree/master/lobiac)
  - [FROS](https://github.com/FunCobal-family/ChestDD_Language/tree/master/fros)

## 設計

サイト自体はIbisUIを用いて構成・記述し、Firebase Hostingでホストする。サーバ側動作はFireBase Runを用いる。

記事はLobiacを使って管理する。ファイルリソースはFROS(File Resource Object Structure)を用いてFireBase FireStoreで保存する

記事は大まかなグループにのみ基づいて出しわけるため記事編集保存時に事前レンダリングしておく。
認証とグループ識別はFireBase Authentificationを用いて行う。

- public
- dev-pack
- democist
- nu
- private
- etc...
