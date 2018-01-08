## Document

***

- Laravel(ローカルプロジェクト)を開始するまで

    - winidowsの場合はbrew,homebrew,curlが利用できないのでComposer(広義パッケージマネージャ)を利用してLaravelを開始する

    - Composerのインストール方法

        - [phpをインストール](http://windows.php.net/download) - 環境パスに通す php.iniに変更

    - インストール

        - `echo @php "%~dp0composer.phar" %*>composer.bat`

        - `php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"`

        - `php composer-setup.php`

    - 不要なフォルダをアンインストール

        - `php -r "unlink('composer-setup.php');"`

    - 動作確認

        - composer -V php --version

    - Laravelプロジェクト

        - Composerを利用してLaravelライブラリをローカルに構築する

        - 親ディレクトリに移動する

        - `composer create-project laravel/laravel プロジェクト名 --prefer-dist` - 7分かかった

    - 動作確認

        - `php artisan serve` `localhost:8000`にアクセスするとLaravel Officelが表示される

    - Laravelフレームワークの概要

        - 201817ディレクトリ `document.md`参照

    




    