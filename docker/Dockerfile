FROM openjdk:17-jdk-slim-bullseye

RUN apt update \
	&& apt install -y default-jre graphviz npm locales \
	&& apt clean -y \
  && cp -p /etc/localtime /etc/localtime.org \
  && ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
  && locale-gen ja_JP.UTF-8 && localedef -f UTF-8 -i ja_JP ja_JP.UTF-8

ENV TZ       Asia/Tokyo
ENV LANGUAGE ja_JP:ja
ENV LC_ALL   ja_JP.utf8
ENV LANG     ja_JP.UTF-8
