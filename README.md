# MakerBot Desktopのインストール 

### 1.リポジトリの追加
```bash
$ sudo apt-add-repository 'http://downloads.makerbot.com/makerware/ubuntu'
```

### 2.サインインkeyの追加
サインインkeyを追加することでUbuntuに信頼のあるソフトウェアであることを信頼させる。
追加しないとインストールまたはアップグレードを確認するメッセージが表示され、自動更新ツールが正常に動作しない場合がある。  
インストールに必要な公開鍵をウェブサイトからダウンロードする
```
$ wget http://downloads.makerbot.com/makerware/ubuntu/dev@makerbot.com.gpg.key
```
keyをダウンロードしたらの次のコマンドでキーリングに追加する。
キーリングに追加することでOSにログインするパスワードを聞かれることをなくす。
```bash
$ sudo apt-key add dev@makerbot.com.gpg.key
```

### 3.ソフトウェアの更新
```bash
$ sudo apt-get update
```

### 4.インストール
```bash
$ sudo apt-get install makerware
```

### 5.makerwareの起動
```bash
$ makerware
```

## その他

#### MakerWareが最新版でない場合
```bash
$ sudo apt-get update
$ sudo apt-get upgrade
```
#### ubuntu 12.04を使っている場合
```bash
$ uname -r
```

#### Maker Desktopのバージョンが3.8以下の場合
```bash
$ sudo apt-get install linux-image-generic-lts-raring
```

**公式サイト**: [https://www.makerbot.com/support/new/04_Desktop/Knowledge_Base/How_to_Install_MakerBot_Desktop_for_Linux](https://www.makerbot.com/support/new/04_Desktop/Knowledge_Base/How_to_Install_MakerBot_Desktop_for_Linux)


