FROM node:alpine as app
# Expose env host
# This is needed to ensure communication between containers
# between docker containers
# Already defined in package.json
ENV HOST 0.0.0.0
ENV PORT 3333

WORKDIR /usr/src

# Run server app
# Detect whether you have a yarn.lock already and if so
# just install deps listed on lock file
# CMD yarn $([ -f yarn.lock ] && echo "install") && $(yarn bin)/nuxt dev
CMD yarn dev