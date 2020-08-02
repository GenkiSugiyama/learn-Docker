# DockerHubからプルするベースとなるimageをFROMで指定
FROM ubuntu:latest
# ENTRYPOINT
# docker run時のデフォルトコマンドを指定できる
# CMDとの違い：ENTRYPOINTのコマンドはdocker run時に上書きできない
# ENTRYPOINTとCMDの両立
# ENTRYPOINTデフォルトコマンドを指定しCMDでそのコマンドのオプションを指定する
# 上記の場合、docker run時で上書きできるのはCMDで指定したデフォルトコマンドの「オプション」のみ
RUN touch test
ENTRYPOINT ["ls"]
CMD ["--help"]