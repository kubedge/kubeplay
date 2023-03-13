FROM alpine:3.17

ENV OPERATOR=/usr/local/bin/kubeplay \
    USER_UID=1001 \
    USER_NAME=kubeplay

# install operator binary
COPY build/_output/bin/kubeplay ${OPERATOR}

COPY build/bin /usr/local/bin

RUN  /usr/local/bin/user_setup

ENTRYPOINT ["/usr/local/bin/entrypoint"]

USER ${USER_UID}
