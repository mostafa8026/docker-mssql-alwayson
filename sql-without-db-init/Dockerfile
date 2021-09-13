FROM mcr.microsoft.com/mssql/server:2019-latest

COPY . /
USER root

RUN /opt/mssql/bin/mssql-conf set sqlagent.enabled true
RUN /opt/mssql/bin/mssql-conf set hadr.hadrenabled  1

CMD /bin/bash ./entrypoint.sh
