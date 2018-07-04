# LINE-LIKE Chat
LINEのような外観のリアルタイムチャットです．  
[動いている様子の動画](https://www.youtube.com/watch?v=RMNYSqGwhMU)

[こちらのURL](https://friendlychat-28f70.firebaseapp.com/)にて動作中です．PCおよびAndroid端末での動作を確認しています．   

## 使い方
1. Firebase CLIをインストール
```
npm install -g firebase-tools
firebase login
```
2. [Firebase Console](https://console.firebase.google.com)上でプロジェクトを作成
3. Authenticationからログイン方法として「Google」「匿名」を有効化
5. Firebase CLIからテスト/デプロイ
```
$ cd LINE-LIKE_Chat
$ firebase use --add
## ここで予め作成したプロジェクトを選択

## テスト用ローカルサーバを起動
$ firebase serve

## デプロイ
$ firebase deploy
```

## 動作説明
### ログイン
発言の投稿・閲覧にはログインが必要です．  
Googleアカウントによるログインに加えて，匿名ユーザーでのログインが可能です．

### 発言
テキストおよび画像の投稿が行えます．  
ログインユーザー自身の発言は右寄せかつ緑色の背景で表示されます．

### 実装について
[Firebase Web Codelab](https://codelabs.developers.google.com/codelabs/firebase-web/)のチュートリアルで作成したFriendly Chatを基に作成しました．


## ライセンス
フォーク元のApache License 2.0に基づきます．  
[LICENSE](LICENSE)を参照してください．