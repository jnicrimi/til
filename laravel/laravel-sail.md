# Laravel Sail

## Install

`curl -s https://laravel.build/sample-app | bash`

## コンテナの起動

`./vendor/bin/sail up -d`

## コンテナの停止

`./vendor/bin/sail stop`

## バージョンの確認

`./vendor/bin/sail version`

## DB

`./vendor/bin/sail exec mysql mysql -u sail -p`
