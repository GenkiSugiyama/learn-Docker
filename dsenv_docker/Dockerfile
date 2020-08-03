FROM ubuntu:latest
# anaconda3をコンテナ内にインストールするためのコマンド
RUN apt-get update && apt-get install -y \
        sudo \
        wget \
        vim
WORKDIR /opt
# 下のRUNコマンドは && でつなげているが最初は一つ一つdocker build→docker runでコンテナ内に入ってどういう処理が必要かを確認しながら
# コマンドをDockerfiに追加していく
RUN wget https://repo.continuum.io/archive/Anaconda3-2019.10-Linux-x86_64.sh && \
    sh Anaconda3-2019.10-Linux-x86_64.sh -b -p /opt/anaconda3 && \
    rm -f Anaconda3-2019.10-Linux-x86_64.sh
ENV PATH /opt/anaconda3/bin:$PATH
RUN pip install --upgrade pip
WORKDIR /
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--allow-root", "--LApp.token=''"]