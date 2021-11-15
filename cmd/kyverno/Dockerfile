FROM gcr.io/distroless/static
ARG TARGETPLATFORM
LABEL maintainer="Kyverno"

ADD ./kyverno-$(echo ${TARGETPLATFORM} | cut -d / -f2) /kyverno

USER 10001

ENTRYPOINT ["./kyverno"]
