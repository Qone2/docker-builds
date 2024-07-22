FROM redis:latest
COPY ./redis.conf /usr/local/etc/redis/redis.conf
COPY ./sentinel.conf /usr/local/etc/redis/sentinel.conf
EXPOSE 6381
EXPOSE 5002
ENTRYPOINT ["sh", "-c"]
CMD ["redis-server /usr/local/etc/redis/redis.conf & redis-sentinel /usr/local/etc/redis/sentinel.conf"]
# docker build -t mysuperimage -f MyDockerfile .
# docker build -t redis-server2 -f redis-server2/Dockerfile redis-server2
# docker run -d --name redis-server2 redis-server2
# docker run -d --name redis-server2 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server2/:/data/ redis-server2
