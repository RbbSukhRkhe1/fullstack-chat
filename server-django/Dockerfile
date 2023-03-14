# syntax=docker/dockerfile:1
   
FROM node:18-alpine
WORKDIR /server-django
COPY . .
RUN yarn install --production
CMD ["pip" "install" "-r" "requirements.txt"]
CMD ["./manage.py" "runserver 0.0.0.0:3001"]

EXPOSE 3001
