# このディレクトリは、PHPのコードの自動整形ツール（PHP Coding Standards Fixer）を実行するのに必要なツールを格納しています。

## 概要

PHP Coding Standards Fixer を使って、PHPのソースコードを自動的に整形します。

## ソースコードの自動整形の実行方法

### 前提条件

* PHP5.3.6以上がインストールされていること

### 使い方

#### dry-run

dry-runPhpCsFixer.sh を、整形したいファイルを引数にして実行すると、どのように整形されるかが標準出力に表示されます。

例：

```bash
./dry-runPhpCsFixer.sh ../../controllers/gnavi_gift/Input.php
```

出力例：

```php
      - public function index() {
      +    public function index()
      +    {
```

引数を指定しないと、対象とすべき全てのディレクトリが指定されます。詳細は、.php_cs.dist を参照してください。

#### run

runPhpCsFixer.sh を、整形したいファイルを引数にして実行すると、ファイルを整形して上書き保存します。対象ファイル自体を上書きしてしまうので注意してください。

引数を指定しないと、対象とすべき全てのディレクトリが指定されます。詳細は、.php_cs.dist を参照してください。
