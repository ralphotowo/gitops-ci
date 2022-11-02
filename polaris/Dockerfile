FROM alpine:3.10

ENV PATH "$PATH:/polaris"

RUN apk add --no-cache bash ca-certificates curl wget tar jq

RUN curl -LJ -o polaris.tar.gz https://github.com/FairwindsOps/polaris/releases/download/5.0.0/polaris_linux_amd64.tar.gz \
    && mkdir polaris \
    && tar -xzf polaris.tar.gz -C polaris 

CMD ["polaris"]
