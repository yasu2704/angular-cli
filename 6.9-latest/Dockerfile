FROM node:6.9
MAINTAINER yasu2704
RUN curl -o- -L https://yarnpkg.com/install.sh | bash \
    && ln -s /root/.yarn/bin/yarn /usr/local/bin/yarn \
    && npm install -g @angular/cli rxjs@^5.0.1
EXPOSE 4200
CMD tail -f /dev/null
