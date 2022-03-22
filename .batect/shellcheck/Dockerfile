FROM koalaman/shellcheck-alpine@sha256:6d8d0884d0bc587526a7e28fdb6bb4dd4afd9c958afaf57f2284e71ebf988493

RUN apk add --no-cache \
    bash=5.1.16-r0

COPY run-shellcheck /usr/local/bin
