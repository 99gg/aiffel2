# Database

```sh
# 도커 컴포즈를 실행하여 postgresql 을 실행한다.
docker compose up -d


# container shell 접속. 이때 컨테이너 이름은 docker-compose.yml에 postgres1234로 설정되어있다.
docker exec -it postgres1234 sh

# postgresql 접속한다.
psql -U postgres
```

```psql
\list
```

![postgres database list](image.png)

```psql
\c postgres
```

![connect to postgres](image-1.png)

```psql
select * from users;
```

![alt text](image-2.png)
