FROM            redhat/ubi9
COPY            mongod.repo /etc/yum.repos.d/mongo.repo
RUN             dnf install mongodb-mongosh git -y
RUN             mkdir /app
WORKDIR         /app
COPY            *.js run.sh  /app/
ENTRYPOINT      ["bash", "run.sh"]