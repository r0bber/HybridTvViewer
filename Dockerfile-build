FROM node:latest

ARG GIT_COMMIT=unknown
LABEL git-commit=$GIT_COMMIT

# Add project files
ADD src /opt/project/src
ADD package.json /opt/project/package.json
ADD webpack.config.js /opt/project/webpack.config.js

WORKDIR /opt/project
RUN npm i
CMD ["bash", "-l", "-c", "npm run build"]

