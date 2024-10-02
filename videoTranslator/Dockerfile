FROM ubuntu:focal

RUN apt update && \ 
    apt install ffmpeg -y && \
    apt install python3 -y && \
    apt install python3-pip -y && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

RUN pip install -U openai-whisper
RUN pip install setuptools-rust

ENTRYPOINT [ "bash" ]