FROM gcr.io/distroless/static
ARG TARGETPLATFORM
LABEL maintainer="Kyverno"

ADD ./kyvernopre-${TARGETPLATFORM} /kyvernopre

USER 10001

ENTRYPOINT ["./kyvernopre"]
