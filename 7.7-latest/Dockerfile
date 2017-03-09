FROM node:7.7
MAINTAINER yasu2704
RUN curl -o- -L https://yarnpkg.com/install.sh | bash \
    && ln -s /root/.yarn/bin/yarn /usr/local/bin/yarn \
    && npm install -g @angular/cli
EXPOSE 3000
CMD tail -f /dev/null
