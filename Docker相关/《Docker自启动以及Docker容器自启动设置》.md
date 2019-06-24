### Docker自启动以及Docker容器自启动设置

#### 1.docker自启动

```java
sudo systemctl enable docker
sudo systemctl start docker
```

#### 2.docker容器自启动

##### 2.1 docker容器运行时自启动

建议在运行容器时就设置容器自启动

使用 run --restart=always 命令

```java
docker run --restart=always 容器名称或容器ID
```

##### 2.2  docker容器运行后设置自启动

使用 update --restart=always 命令

```java
docker update --restart=always 容器名称或容器ID
```