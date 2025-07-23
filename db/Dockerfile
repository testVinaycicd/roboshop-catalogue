FROM            redhat/ubi9
RUN             dnf install mongodb-mongosh git -y
RUN             mkdir /home/app
WORKDIR         /home/app
COPY            mongod.repo /etc/yum.repos.d/mongo.repo
COPY            *.js run.sh  /app/
ENTRYPOINT      ["bash", "run.sh"]