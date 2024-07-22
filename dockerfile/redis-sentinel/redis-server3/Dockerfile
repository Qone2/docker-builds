FROM redis:latest
COPY ./redis.conf /usr/local/etc/redis/redis.conf
COPY ./sentinel.conf /usr/local/etc/redis/sentinel.conf
EXPOSE 6381
EXPOSE 5002
ENTRYPOINT ["sh", "-c"]
CMD ["redis-server /usr/local/etc/redis/redis.conf & redis-sentinel /usr/local/etc/redis/sentinel.conf"]
# docker build -t mysuperimage -f MyDockerfile .
# docker build -t redis-server3 -f redis-server3/Dockerfile redis-server3
# docker run -d --name redis-server3 redis-server3
# docker run -d --name redis-server3 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server3/:/data/ redis-server3
# docker run -d --name redis-server3 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server3/:/data/ --network bridge redis-server3
# docker run -d --name redis-server3 -v /mnt/c/Users/Qone/repositories/docker/logs/redis-server3/:/data/ --network host redis-server3
# docker run -d --name redis-server3 --network bridge -p 6381:6381 -p 5002:5002 redis-server3
