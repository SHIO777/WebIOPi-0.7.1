# WebIOPi-0.7.1

```bash

wget https://sourceforge.net/projects/webiopi/files/WebIOPi-0.7.1.tar.gz
tar xvzf WebIOPi-0.7.1.tar.gz     #ファイル解凍
cd WebIOPi-0.7.1                  #ディレクトリ移動
wget https://raw.githubusercontent.com/doublebind/raspi/master/webiopi-pi2bplus.patch       #修正プログラムダウンロード
patch -p1 -i webiopi-pi2bplus.patch  #ダウンロードした修正プログラムの適用
sudo ./setup.sh                   #セットアップスクリプトの適用
```

"Do you want to accessWebIOPi over Internet? [y/n]"　で止まったら、"n"を入力し、エンターキーを押す（"y"を入力し、エンターキーを押すと、"Weaved IoT Kit"がインストールされる）。
WebIOPiをサービスとして開始するためのファイルをダウンロードする。

```
cd /etc/systemd/system/
sudo wget https://raw.githubusercontent.com/doublebind/raspi/master/webiopi.service
cd ~   #ホームディレクトリへの移動
```
