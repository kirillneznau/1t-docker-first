1. Чтобы создать образ из dockerfil-а:
docker build -t postgres_bd_img .
2. Чтобы запустить контейнер из образа:
docker run --name postgres_bd_container -p 5432:5432 -d postgres_bd_img
3. Чтобы зайти в интерактивную оболочку внутри контейнера и внести изменения в базу данных:
docker exec -it test psql -U postgres