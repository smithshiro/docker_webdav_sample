# nginx webdav sample

WebDAVの機能を確かめる用

## Getting Started

### Prerequisites

docker version
```
$ docker -v
Docker version 19.03.12, build 48a66213fe
```
docker-compose version
```
$ docker-compose -v
docker-compose version 1.26.2, build eefe0d31
```
### Installing

インストール
```
$ docker-compose up -d
```
## Running the tests
ファイルアップロード

```
curl -v -X PUT -F upfile=sample.jpg http://localhost:10088/sample.jpg
```

ファイルダウンロード

```
curl -v -X GET -o sample2.jpg http://localhost:10088/sample.jpg
```
