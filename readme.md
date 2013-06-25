# 開発用ツールのインストーラです。

## ダウンロード

zip でダウンロードしても良いですが git clone を推奨します。  
好きな場所に配置して下さい。PHP をインストールしてあるドライブと同じが良いと思います。  
PHP にはパスを通しておいて下さい。

以下、仮に D:\php-devtools として配置したとします。  
以下、このディレクトリ直下を"ルート"と呼びます。

## 開発用ツールのインストール

Composer で各パッケージをインストールします。ルートで実行して下さい。

	$ php composer.phar install # 初回
	$ php composer.phar update # 二回目以降

D:\php-devtools\vendor\bin にパスを通します。  
パスを通した後、OSの再起動が必要かもしれません。

### PHPUnit の確認

PHPUnit にパスが通っているか確認します。

	$ which phpunit
	/d/php-devtools/vendor/bin/phpunit

### その他

PHPUnit と同様の場所に

* apigen.php http://apigen.org/
* php-cs-fixer http://cs.sensiolabs.org/

が入っています。

## ライセンス

Copyright 2013, CoreTech Co.,Ltd. Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
