FROM            redhat/ubi9
RUN             dnf install mongodb-mongosh git -y
RUN             mkdir /app
WORKDIR         /app
COPY            mongod.repo /etc/yum.repos.d/mongo.repo
COPY            *.js run.sh  /app/
ENTRYPOINT      ["bash", "run.sh"]