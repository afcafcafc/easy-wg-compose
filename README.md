
sudo mkdir -p /etc/docker/containers/wg-easy


sudo curl -o /etc/docker/containers/wg-easy/docker-compose.yml \
https://raw.githubusercontent.com/afcafcafc/easy-wg-compose/refs/heads/main/docker-compose.yml


cd /etc/docker/containers/wg-easy

sudo docker compose up -d

# 进入目录
cd /etc/docker/containers/wg-easy

# 拉取最新镜像
sudo docker compose pull

# 重新创建容器
sudo docker compose up -d
