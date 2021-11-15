FROM gcr.io/distroless/static
ARG TARGETPLATFORM
RUN export ARCH=$(echo ${TARGETPLATFORM} | cut -d / -f2)
LABEL maintainer="Kyverno"

ADD ./kyverno-$ARCH /kyverno

USER 10001

ENTRYPOINT ["./kyverno"]
