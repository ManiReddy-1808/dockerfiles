FROM almalinux:9
RUN dnf install nginx -y
# Never run containers with root access. It is a security risk. Always create a user and run container with that user.
# By default container will run with root user. We can change it to any other user.
# Required root access to run nginx
RUN useradd roboshop
USER roboshop
# Now container will run with roboshop user.
CMD ["sleep", "100"]