FROM node:16
EXPOSE 5000 3000 80 443
RUN apt-get update && apt-get install -y git
RUN git clone https://gitlab.com/redacre/test-project.git
WORKDIR test-project/sys-stats
RUN npm install
RUN npm run build
CMD ["npm", "start"]