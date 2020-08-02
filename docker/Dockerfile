# DockerHubからプルするベースとなるimageをFROMで指定
FROM ubuntu:latest
# RUN ~ で作成したimageへのコマンドを実行
RUN mkdir /new_dir
# COPYとADDの違いについて
# COPY：ホストのファイルをそのままコンテナにコピーする場合に使用する
# ADD：tarの圧縮ファイルをコンテナにコピーし解凍する場合に使用する
# railsとかをコンテナで動かすときはADDで持っていくのかな？
ADD compressed.tar /