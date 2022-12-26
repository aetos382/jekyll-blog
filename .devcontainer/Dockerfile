FROM ruby:3.1.3-bullseye

RUN echo "gem: --no-ri --no-rdoc" > ~/.gemrc

RUN gem update --system
RUN gem install --force bundler
RUN gem install jekyll -- --use-system-libraries

ENTRYPOINT ["/bin/bash"]

VOLUME /usr/local/bundle/gems

EXPOSE 4000
