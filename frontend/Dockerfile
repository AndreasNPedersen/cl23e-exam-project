
# build stadie
FROM node:lts-alpine as bS
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build

# production stadie
FROM nginx:stable-alpine as pS
COPY --from=bS /app/dist /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]