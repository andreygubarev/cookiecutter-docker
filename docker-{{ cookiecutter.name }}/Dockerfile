# syntax=docker/dockerfile:1
FROM debian:bookworm-slim
LABEL org.opencontainers.image.title="{{ cookiecutter.name }}"
LABEL org.opencontainers.image.description="{{ cookiecutter.description }}"
LABEL org.opencontainers.image.authors="{{ cookiecutter.author }}"

COPY docker-entrypoint.sh /docker-entrypoint.sh
ENTRYPOINT ["tini", "--", "/docker-entrypoint.sh"]
