# LocalStack

## Install

`brew install localstack/tap/localstack-cli`

## awslocal

LocalStack が提供している AWS CLI のラッパー。

### Install

`pip3 install awscli-local`

## 動作検証

### 起動

`localstack start -d`

### 確認

`localstack status services`

### 停止

`localstack stop`

## S3

### バケットの作成

`awslocal s3 mb s3://example-bucket`

#### 確認

`awslocal s3 ls`

### ファイルのアップロード

#### ファイルの作成

`touch example.txt`

#### ファイルのアップロード

`awslocal s3 cp ./example.txt s3://example-bucket/`

#### 確認

`awslocal s3 ls s3://example-bucket1`

### ファイルのダウンロード

#### ローカルファイルの削除

`rm -f example.txt`

#### ファイルのダウンロード

`awslocal s3 cp s3://example-bucket/example.txt ./example.txt`

#### 確認

`ls example.txt`
