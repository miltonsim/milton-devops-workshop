docker build -t sample-vm .
docker run -p 22:22 sample-vm

docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' a54173703884
docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' b2dc6c3928cd 

172.28.0.4
172.28.0.3

ansible -i hosts all -m ping

dry mode --dry-mode

https://localhost:8080/