FROM ruby:3.1.3-bullseye

RUN apt update -y && \
    apt upgrade -y --no-install-recommends && \
    apt install -y --no-install-recommends \
        liblapacke-dev  \
        libopenblas-dev && \
    apt autoremove -y --purge && \
    apt autoclean -y

RUN gem install jekyll

ENTRYPOINT ["/bin/bash"]

VOLUME /usr/local/bundle/gems

EXPOSE 4000
