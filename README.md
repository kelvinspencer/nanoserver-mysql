# nanoserver-mysql
Windows Nanoserver MySQL Docker Repo


docker run --name mysql -d -it -p 3306:3306 spencerfirmllc/nanoserver-mysql \
docker exec -it mysql cmd \
mysql –u root –p \
(MySQL will launch using the root user.) Will prompt for password

Show running containers: docker ps -a -f status=running \
Show container IP: docker inspect -f "{{ .NetworkSettings.Networks.nat.IPAddress }}" mysql \
Show containerID: docker inspect --format="{{.Id}}" mysql \


https://hub.docker.com/r/spencerfirmllc/nanoserver-mysql \
https://hub.docker.com/r/nanoserver/iis-php \
