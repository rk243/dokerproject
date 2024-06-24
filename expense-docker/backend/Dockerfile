FROM nodejs:20
EXPOSE 8080
RUN useradd expense
RUN mkdir /opt/sever
RUN CHOWN expense:expense -R /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.JS .
RUN npm install
CMD [ "node","index.js" ]


