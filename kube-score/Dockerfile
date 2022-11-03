FROM alpine:3.10

ENV PATH "$PATH:/kube-score"

RUN apk add --no-cache bash ca-certificates curl wget tar jq

RUN curl -LJ -o kube-score_1.14.0_linux_amd64 https://github.com/zegl/kube-score/releases/download/v1.14.0/kube-score_1.14.0_linux_amd64 \
    && mkdir /kube-score \
    && mv kube-score_1.14.0_linux_amd64 /kube-score/kube-score \
    && chmod +x /kube-score/kube-score

CMD ["kube-score"]
