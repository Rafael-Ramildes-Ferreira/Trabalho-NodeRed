FROM nodered/node-red:latest

# Install additional nodes
RUN npm install node-red-dashboard

# Expose the default port
EXPOSE 1880

CMD ["npm", "start", "--", "--userDir", "/data"]
