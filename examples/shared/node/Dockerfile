FROM node:21.2-bullseye-slim@sha256:902c76e447930176b432ecf1870c78680e9956adb75be2579f2fd9ac2aa6e46a as node-base


FROM node-base as node-http-auth
ARG NODE_APP=.
ARG NODE_APP_NAME=http-service/server
# Add an env to save ARG
ENV NODE_APP_PATH "/app/${NODE_APP_NAME}"
COPY "$NODE_APP" /app
# Dont use exec form to interpolate correctly
CMD node $NODE_APP_PATH
