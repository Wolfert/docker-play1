FROM openjdk:8
LABEL maintainer="Ludovico Fischer <livrerie@gmail.com>"
RUN groupadd -r play && useradd --no-log-init -r -g play -m play
WORKDIR /home/play
USER play
RUN wget https://downloads.typesafe.com/play/1.5.0/play-1.5.0.zip && unzip play-1.5.0.zip && rm play-1.5.0.zip
ENTRYPOINT ["/home/play/play-1.5.0/play"]
EXPOSE 9000
