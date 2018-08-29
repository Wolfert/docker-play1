FROM openjdk:10
LABEL maintainer="Ludovico Fischer <livrerie@gmail.com>"
RUN groupadd -r play && useradd --no-log-init -r -g play -m play
WORKDIR /home/play
USER play
RUN wget https://downloads.typesafe.com/play/1.5.1/play-1.5.1.zip && unzip play-1.5.1.zip && rm play-1.5.1.zip
ENTRYPOINT ["/home/play/play-1.5.1/play"]
EXPOSE 9000
