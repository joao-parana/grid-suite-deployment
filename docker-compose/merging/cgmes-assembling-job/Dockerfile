FROM gridsuite/cgmes-assembling-job:latest
USER root
ENTRYPOINT []
RUN apt-get clean 
RUN apt-get update --allow-insecure-repositories
RUN apt-get -y install cron
COPY init-job-container.sh /root
CMD chmod a+x /root/init-job-container.sh
CMD /root/init-job-container.sh

