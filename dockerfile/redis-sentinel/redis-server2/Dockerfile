FROM redis:latest
COPY /mnt/c/Users/Qone/repositories/docker/configs/dockerfile/redis-sentinel/redis-server2/redis.conf /usr/local/etc/redis/redis.conf
COPY /mnt/c/Users/Qone/repositories/docker/configs/dockerfile/redis-sentinel/redis-server2/sentinel.conf /usr/local/etc/redis/sentinel.conf
RUN redis-server /usr/local/etc/redis/redis.conf
RUN redis-sentinel /usr/local/etc/redis/sentinel.conf
EXPOSE 6380
EXPOSE 5001
# docker run -d --name redis-server2 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server2/:/var/log/redis/ redis-server2
