# 環境構築

Windows上で色んな環境の構築方法についてのまとめ

極力, `WSL`は利用しない構築方法にする。

## Python
pythonのバージョンは
pyenv を利用してバージョンコントロールする

パッケージ管理は`poetry`を利用する

詳しくは[こちら](/python/README.md)


## WebApp

以下の環境を使った環境構築

- nuxt.js
- postgresql
  - とりあえずdocker-composeを利用
  - 後ほどネイティブにインストールする作業を記述する

TO-DO:
以下のインストール仕方
- node
- npm
- yarn
- postgresql
- CosmoDB: local
  - とりあえずdocker-composeを利用

## Reference
[ちゃんと理解するrbenv : (4) shimsを理解する](https://mogulla3.tech/articles/2021-07-12-understanding-rbenv-4)  
[What is a Shim?](https://stackoverflow.com/questions/2116142/what-is-a-shim)
