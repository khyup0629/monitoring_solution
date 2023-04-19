# monitoring_solution

> <h3>docker 설치</h3>

- 구성환경 : AWS
- OS : Amazon Linux 2

```bash
# yum update
# yum install docker -y
# docker -v
# service docker start 
```

## docker-compose 설치

```bash
# curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
# chmod +x /usr/local/bin/docker-compose
```

## EBS 볼륨 인스턴스에 추가(/data에 마운트)

=> https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/ebs-using-volumes.html

```bash
# mkdir -p /data/influxdb/config
# mkdir -p /data/influxdb/data
# mkdir -p /data/grafana/etc_grafana
# mkdir -p /data/grafana/var_lib_grafana
# mkdir -p /data/telegraf/
# chown -R 472:472 /data/grafana/
```

