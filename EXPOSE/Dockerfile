FROM almalinux:9
RUN dnf install nginx -y
EXPOSE 80
# Just giving the info to user to expose container port on this
CMD ["nginx","-g","daemon off;"]