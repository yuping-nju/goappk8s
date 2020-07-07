FROM golang:latest
WORKDIR $GOPATH/src/github.com/yuping-nju/ping
ADD . $GOPATH/src/github.com/yuping-nju/ping
RUN go env -w GO111MODULE=on
RUN go env -w GOPROXY=https://goproxy.cn,direct
RUN go install .
CMD [ "ping" ]

