FROM gcr.io/distroless/static

ARG TARGETPLATFORM

LABEL maintainer="Kyverno"

ADD ./kyvernopre-${echo $TARGETPLATFORM | cut -d / -f2} /kyvernopre

USER 10001

ENTRYPOINT ["./kyvernopre"]
