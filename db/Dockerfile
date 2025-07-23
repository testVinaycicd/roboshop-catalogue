FROM            redhat/ubi9
COPY            mongod.repo /etc/yum.repos.d/mongo.repo
RUN             dnf install mongodb-mongosh git -y
RUN             mkdir /home/app
WORKDIR         /home/app
COPY            *.js run.sh  /app/
ENTRYPOINT      ["bash", "run.sh"]