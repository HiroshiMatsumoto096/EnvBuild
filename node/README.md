# node

## `nvm-windows`

`node.js`のバージョン管理ツール  
https://github.com/coreybutler/nvm-windows

`node.js`をwindowsで動かすのが大変である.  
`node.js`本家が各バージョンのインストーラーを提供しているが、  
更新されたら都度ダウンロード/インストール作業が必要となる。  
https://nodejs.org/ja

`docker-compose`でも行えるが`docker`は重い.  

そのため、`nvm`でnodeのバージョン管理を行うのが理想的.  

## インストール手順

以下より最新版の`nvm-windows`をダウンロードし、インストールを進める.  
https://github.com/coreybutler/nvm-windows/releases

利用可能な`node`バージョンを確認  

```
nvm install available
```
(20.5.1最新, 20203/08/30現在)  

`nvm`を使って最新版の`node.js`インストール  

```
nvm install latest
```
`latest`と書くだけで最新版が導入される.  
バージョン番号指定してもOK.  
例: `nvm install 20.5.1`

`node.js`をインストールすると`npm`も同時ダウンロードされる.  
`yarn`はダウンロードされないので別途ダウンロードが必要.  

利用する`node`バージョンを指定..   
そのフォルダ以下は別に指定がされていなければ、このバージョンになる  
```
nvm use 20.5.1
```

`yarn`のインストール

```
npm install yarn --save --legacy-peer-deps
```

*) オプション付けないと動かなかった
```
--save --legacy-peer-deps
```
https://qiita.com/koh97222/items/c46d1ef2a63b92bb6c15
