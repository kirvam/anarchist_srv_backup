FROM perl:latest

MAINTAINER Paul Haigh (Natalia Strelkova) pmphaigh@gmail.com

RUN curl -L http://cpanmin.us | perl - Dancer2
RUN cpanm Starman
#RUN no_cache=2015-09-01 git clone https://github.com/skalolazka/dancer-playground.git
RUN git clone https://github.com/kirvam/Flore-DancerPlayground.git


EXPOSE 5001

WORKDIR Flore-DancerPlayground/Flore-DancerPlayground

CMD starman --port 5001 bin/app.psgi

