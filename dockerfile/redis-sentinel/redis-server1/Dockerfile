FROM redis:latest
COPY ./redis.conf /usr/local/etc/redis/redis.conf
COPY ./sentinel.conf /usr/local/etc/redis/sentinel.conf
EXPOSE 6379
EXPOSE 5000
ENTRYPOINT ["sh", "-c"]
CMD ["redis-server /usr/local/etc/redis/redis.conf & redis-sentinel /usr/local/etc/redis/sentinel.conf"]
# docker run -d --name redis-server1 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server1/:/data/ redis-server1
