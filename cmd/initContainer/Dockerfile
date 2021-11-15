FROM gcr.io/distroless/static

ARG TARGETPLATFORM

ENV ARCH=$(echo ${TARGETPLATFORM} | cut -d / -f2)

LABEL maintainer="Kyverno"

ADD ./kyvernopre-${ARCH} /kyvernopre

USER 10001

ENTRYPOINT ["./kyvernopre"]
