# PHPによるWebアプリケーションスーパーサンプル活用編
---
## 実行環境
* OS windows7
* xampp version 5.6.8
---
## pear パッケージ & 必要なインストール物
* MDB2
    * pear install --alldeps MDB2-2.5.0b5
* MDB2_Driver_mysql
    * pear install --alldeps MDB2_Driver_mysql-1.5.0b4
* smarty
    * https://github.com/smarty-php/smarty/releases/tag/v3.1.24
    * ディレクトリ名「smarty」に変更
* HTML_QuickForm2
    * pear install --alldeps HTML_QuickForm2-2.0.2
    * smarty用拡張モジュール「HTML_QuickForm2_Renderer_Smarty」のインストール
* php-google-map-api
    * https://github.com/streetlogics/php-google-map-api 3.0
    * ※GoogleMap.php と JSMin.phpが必要（修正する必要あり）
    * ディレクトリ名「gmaps」作成して配置
* facebook php sdk v5.0
    * https://developers.facebook.com/docs/php/gettingstarted/5.0.0
    * ディレクトリ名「facebook-php-sdk-v4-5.0-dev」で配置
*　twitteroauth
    * https://github.com/abraham/twitteroauth
    * ディレクトリ名「twitteroauth」で配置

* ※上記ファイル郡すべてpearフォルダに入れます。

共有フォルダ内にpearインストール以外のものを用意してます。
※smarty用拡張モジュール「HTML_QuickForm2_Renderer_Smarty」のみ設置場所は「pear/HTML/QuickForm2/Renderer」内に設置

---
## 設定
* hostsファイルのlocalhost名に「kurumadani.com」を追加
* my.ini 追記
    * [mysqld]
    * character-set-server=utf8
    *  skip-character-set-client-handshake
    *  [mysql]
    *  default-character-set=utf8
* php-google-map-api
    * googleMap.php 内コード修正
    * ファイル　php_super_sample/Chapter7/　に用意してます。
---
## その他
- データベース
    - github php_super_sample/Chapter7/ の「addbook_db.sql」使用
