# vagrant_puppeteer
Vagrant を用いて Ubuntu 20.04 に puppeteer と headless Chrome をインストールします。

## puppeteer
* puppeteer と headless Chrome をインストールします。
* 日本語フォントをインストールします。
* タイムゾーンを JST に設定します。
### 事前にインストールするソフトウェア
* VirtualBox
* Vagrant
* vagrant plugin install vagrant-proxyconf (proxy使用時)
* vagrant plugin install vagrant-vbguest (オプション)

### インストール
必要に応じてhttp_proxy, https_proxyの環境変数を設定してください。
vagrant up を実行し VM を作成します。

    $ vagrant up

vagrant ssh を実行し VM にログインします。

    $ vagrant ssh

puppeteerで実行したい内容をファイル(例: sample.js ) に記載し、 sample.js を実行します。

    $ node sample.js

### 参考
* https://medium.com/@oofnivek/ubuntu-install-puppeteer-bd551d6e5fc1
* https://doruby.jp/users/nakamatsu/entries/puppeteer-%E3%81%A7-Headless-%E3%81%97%E3%81%A6%E3%81%BF%E3%81%9F
* https://qiita.com/teruroom/items/d6c79ee1a99a3d57f788
* https://qiita.com/kanoe/items/9043a81d28a1b733b2e2

### ToDo
- ドキュメント
