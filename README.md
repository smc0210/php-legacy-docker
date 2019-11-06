# php:5.6-fpm, nginx, mysql

## Requirements

- docker >= 19.03 (docker for mac)
- npm or yarn

## Installation

```bash
cp .env_example .env
```

.env 파일을 생성한 후 환경변수를 작성합니다.

```
PROJECT_PATH=../프로젝트경로
HOST_HTTP_PORT=8080
HOST_MYSQL_PORT=3307
MYSQL_DATABASE=schema이름
MYSQL_USER=root
MYSQL_PASSWORD=1234
```

## Usage

```bash
yarn start
yarn down
```
