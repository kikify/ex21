FROM python:3.8-slim

#作業ディレクトリを変更
WORKDIR /tmp/mydir

#ファイルのコピー
COPY requirements.txt ${PWD}

#pythonのパッケージをインストール
RUN pip install -r requirements.txt

#一次変数の定義
ARG wdir

#作業ディレクトリを変更
WORKDIR $wdir