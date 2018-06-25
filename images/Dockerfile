FROM jenkins/jenkins:lts
COPY plugins.txt /plugins.txt
RUN /usr/local/bin/install-plugins.sh $(cat /plugins.txt | tr '\n' ' ')
#RUN /usr/local/bin/plugins.sh /plugins.txt 
