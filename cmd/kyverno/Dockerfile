FROM gcr.io/distroless/static
ARG TARGETPLATFORM
LABEL maintainer="Kyverno"

ADD ./kyverno-${TARGETPLATFORM} /kyverno

USER 10001

ENTRYPOINT ["./kyverno"]
