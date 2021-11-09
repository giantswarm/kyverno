FROM alpine:3.14.2 AS builder

LABEL maintainer="Kyverno"

RUN apk add --no-cache ca-certificates

# Packaging stage
FROM scratch

LABEL maintainer="Kyverno"
ADD ./kyverno /kyverno
COPY --from=builder /etc/ssl/certs/ca-certificates.crt /etc/ssl/certs/

USER 10001

ENTRYPOINT ["./kyverno"]
