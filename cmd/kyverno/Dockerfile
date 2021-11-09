FROM gcr.io/distroless/base

LABEL maintainer="Kyverno"

ADD ./kyverno /kyverno

USER 10001

ENTRYPOINT ["./kyverno"]
