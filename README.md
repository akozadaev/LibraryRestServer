# LibraryRestServer

Написано для проекта школы Samsung

запуск ```go run main.go```

слушает порт 8000

Методы:

1. [GET]/books - список всех книг и информация по ним
2. [GET]/books/{id} - информация по книги с указанным id
3. [POST] /books - добавление информации по новой книге 
4. [PUT] /books/{id} - корректировка информации по книги с указанным id
5. [DELETE]/books/{id}- удаление информации по книги с указанным id

Работает без БД, поэтому после запуска есть информация только по двум книгам. Хард 

6. [POST] /file - загрузка файла
curl -X POST \
http://localhost:8080/file \
-H 'Accept: */*' \
-H 'Accept-Encoding: gzip, deflate' \
-H 'Cache-Control: no-cache' \
-H 'Connection: keep-alive' \
-H 'Content-Length: 4251' \
-H 'Content-Type: multipart/form-data; boundary=--------------------------489143350034706567613009' \
-H 'Host: localhost:8081' \
-H 'Postman-Token: fea94e80-8294-4f0b-87bf-09b706eddac8,1bbb735b-f88d-4194-a1b5-f8cd90189545' \
-H 'User-Agent: PostmanRuntime/7.17.1' \
-H 'cache-control: no-cache' \
-H 'content-type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW' \
-F file=@/home/users/akozadaev/book.txt \
-F file_name=file1