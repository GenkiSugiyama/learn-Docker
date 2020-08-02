# DockerHubからプルするベースとなるimageをFROMで指定
FROM ubuntu:latest
# RUN ~ で作成したimageへのコマンドを実行
# 実行コマンドを&&で繋げることでRUNコマンド1つで複数のインストラクションを実行できる
RUN apt-get update && apt-get install -y \
    curl \
    cvs \
    nginx
CMD ["ls"]