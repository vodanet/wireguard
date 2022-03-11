
FROM nginx
RUN apt-get update
RUN apt-get install net-tools -y
RUN apt-get install vim -y
RUN mkdir ./data
COPY ./mbvdmonitoring_1.0.0_amd64.deb ./data/mbvdmonitoring_1.0.0_amd64.deb
COPY ./mbvdmonitoring_1.0.0_amd64.deb ./data/mbvdmonitoring_1.0.0_amd64.deb
RUN dpkg -i data/mbvdmonitoring_1.0.0_amd64.deb
RUN apt-get install -f ./data/mbvdmonitoring_1.0.0_amd64.deb
RUN echo "" > ~/.bash_history
