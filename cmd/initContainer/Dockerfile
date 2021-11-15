ARG ARCH=

FROM gcr.io/distroless/static

LABEL maintainer="Kyverno"

ADD ./kyvernopre-${ARCH} /kyvernopre

USER 10001

ENTRYPOINT ["./kyvernopre"]
