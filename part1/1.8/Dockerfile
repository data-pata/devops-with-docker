FROM ubuntu:20.04

WORKDIR /usr/src/app

COPY echo.sh .

RUN --mount=type=cache,target=/var/cache/apt,sharing=locked \
  --mount=type=cache,target=/var/lib/apt,sharing=locked \
  apt update && apt-get --no-install-recommends install -y curl

CMD ./echo.sh