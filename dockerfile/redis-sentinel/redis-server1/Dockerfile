FROM redis:latest
COPY ./redis.conf /usr/local/etc/redis/redis.conf
COPY ./sentinel.conf /usr/local/etc/redis/sentinel.conf
EXPOSE 6379
EXPOSE 5000
ENTRYPOINT ["sh", "-c"]
CMD ["redis-server /usr/local/etc/redis/redis.conf & redis-sentinel /usr/local/etc/redis/sentinel.conf"]
# docker build -t mysuperimage -f MyDockerfile .
# docker build -t redis-server1 -f redis-server1/Dockerfile redis-server1
# docker run -d --name redis-server1 redis-server1
# docker run -d --name redis-server1 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server1/:/data/ redis-server1
# docker run -d --name redis-server1 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server1/:/data/ --network bridge redis-server1
# docker run -d --name redis-server1 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server1/:/data/ --network host redis-server1
# docker run -d --name redis-server1 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server1/:/data/ -p 6379:6379 --network host redis-server1
# docker run -d --name redis-server1 --network host redis-server1
# docker run -d --name redis-server1 --network bridge -p 6379:6379 -p 5000:5000 redis-server1
