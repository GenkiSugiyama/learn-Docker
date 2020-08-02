# DockerHubからプルするベースとなるimageをFROMで指定
FROM ubuntu:latest
# RUN ~ で作成したimageへのコマンドを実行
RUN mkdir /new_dir
# COPYはRUNと同様イメージレイヤーを作るので書きすぎは注意？
COPY something /new_dir/