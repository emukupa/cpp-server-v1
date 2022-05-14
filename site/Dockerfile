FROM emukupa/ubuntu-bionic:v1

WORKDIR /usr/src
COPY . .
RUN cmake . && make
CMD ["./initiate_site"]
