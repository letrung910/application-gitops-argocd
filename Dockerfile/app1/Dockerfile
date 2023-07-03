# docker build -t test . --build-arg ENVIRONMENT=dev  --build-arg COMMIT_HASH=123123
FROM nginx:stable-alpine
ARG ENVIRONMENT=dev1
ARG COMMIT_HASH
COPY index.html /usr/share/nginx/html/index.html
RUN echo "${ENVIRONMENT}-app1:${COMMIT_HASH}" >> /usr/share/nginx/html/index.html

