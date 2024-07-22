FROM redis:latest
COPY ./redis.conf /usr/local/etc/redis/redis.conf
COPY ./sentinel.conf /usr/local/etc/redis/sentinel.conf
EXPOSE 6380
EXPOSE 5001
ENTRYPOINT ["sh", "-c"]
CMD ["redis-server /usr/local/etc/redis/redis.conf & redis-sentinel /usr/local/etc/redis/sentinel.conf"]
# docker build -t mysuperimage -f MyDockerfile .
# docker build -t redis-server2 -f redis-server2/Dockerfile redis-server2
# docker run -d --name redis-server2 redis-server2
# docker run -d --name redis-server2 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server2/:/data/ redis-server2
# docker run -d --name redis-server2 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server2/:/data/ --network bridge redis-server2
# docker run -d --name redis-server2 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server2/:/data/ --network host redis-server2
# docker run -d --name redis-server2 --network bridge -p 6380:6380 -p 5001:5001 redis-server2
