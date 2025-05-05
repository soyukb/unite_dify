FROM nvidia/cuda:12.8.0-runtime-ubuntu22.04

# 事前にcurlをインストール
RUN apt update && apt install -y curl

# ollamaのインストールスクリプトを取得して実行
RUN curl -fsSL https://ollama.com/install.sh | sh

# コンテナ実行時のコマンド
CMD ["/bin/sh", "-c", "ollama serve"]