# インストール有無を確認

まずは、Composerがインストール済みかを確認する。
以下のパスが存在するか確認する。

```
/usr/local/bin/composer
```

パスを通っているならコマンドでも確認できる。

```
$ composer -V
```

# インストールする①

公式サイトの方法をそのまま行う。( [公式サイト](https://getcomposer.org/download/) )

```text
$ php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
$ php -r "if (hash_file('SHA384', 'composer-setup.php') === trim(file_get_contents('https://composer.github.io/installer.sig'))) { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
$ php composer-setup.php
$ php -r "unlink('composer-setup.php');"
```

# インストールする②

インストール済みでなかったら、以下のコマンドを実行する。

```
$ curl -sS https://getcomposer.org/installer | php
$ mv composer.phar /usr/local/bin/composer
```

# 参考記事

[LinuxでPHPのcurlをインストール・有効化する方法](https://zukucode.com/2017/09/php-curl-install.html)  