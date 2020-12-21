ENV USER user1

#一般権限のユーザーを追加
RUN useradd -m ${USER}
#sudoの権限を付与
RUN gpasswd -a ${USER} sudo
#パスワード設定
RUN echo "${USER}:pass" | chpasswd

#ユーザーの切替
USER ${USER}
