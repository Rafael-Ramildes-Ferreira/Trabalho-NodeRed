FROM nodered/node-red:latest

# Install additional nodes
RUN npm install node-red-dashboard node-red-contrib-web-worldmap node-red-contrib-aedes

# Expose the default port
EXPOSE 1880

CMD ["npm", "start", "--", "--userDir", "/data"]
