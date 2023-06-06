FROM almalinux
RUN yum install nginx -y
# The below command will not execute when the creator of this command is running. But executes when some other people using this image.
ONBUILD ADD simple.txt /tmp/