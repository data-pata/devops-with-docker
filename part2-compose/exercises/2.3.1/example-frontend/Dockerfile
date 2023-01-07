FROM node:16

WORKDIR /usr/src/app/

# Copy and install deps to cache them before project build.
COPY package*.json ./

RUN npm ci --only=production
RUN npm install -g serve

COPY . . 

ENV REACT_APP_BACKEND_URL=http://localhost:8080
RUN npm run build


EXPOSE 5000
CMD ["serve", "-s", "-l", "5000", "build"]
