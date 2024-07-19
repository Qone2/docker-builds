FROM redis:latest
COPY /mnt/c/Users/Qone/repositories/docker/configs/dockerfile/redis-sentinel/redis-server3/redis.conf /usr/local/etc/redis/redis.conf
COPY /mnt/c/Users/Qone/repositories/docker/configs/dockerfile/redis-sentinel/redis-server3/sentinel.conf /usr/local/etc/redis/sentinel.conf
RUN redis-server /usr/local/etc/redis/redis.conf
RUN redis-sentinel /usr/local/etc/redis/sentinel.conf
EXPOSE 6381
EXPOSE 5002
# docker run -d --name redis-server3 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server3/:/var/log/redis/ redis-server3
