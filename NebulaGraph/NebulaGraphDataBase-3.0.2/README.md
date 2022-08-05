1. 启动Nebula集群

   ``` shell
   docker-compose up -d
   ```

2. 连接Nebula集群

   ```shell
   docker run --rm -ti --network nebula-docker-compose-master_nebula-net --entrypoint=/bin/sh vesoft/nebula-console:v3.0.0
   ```

   检查network

   ``` shell
   docker network ls
   ```

3. 连接Nebula实例

    ``` shell
    nebula-console -u root -p 123 --address=graphd --port=9669
    ```

4. 基本使用方式详见官网
