FROM ubuntu:20.04

WORKDIR /usr/src/app

LABEL dwd=1.8

RUN --mount=type=cache,target=/var/cache/apt,sharing=locked \
  --mount=type=cache,target=/var/lib/apt,sharing=locked \
  apt-get update && apt-get --no-install-recommends install -y curl

COPY echo.sh .

ENTRYPOINT ["./echo.sh"]
