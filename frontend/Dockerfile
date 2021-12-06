FROM node as builder
RUN git clone https://github.com/asilnikov/docker_homework.git
WORKDIR ./docker_homework/frontend
RUN npm install
ENV NODE_OPTIONS=--openssl-legacy-provider
RUN npm run build

FROM node:fermium-alpine3.14
RUN npm install -g serve
COPY --from=builder ./docker_homework/frontend/build ./build
CMD ["serve", "-s", "build"]
