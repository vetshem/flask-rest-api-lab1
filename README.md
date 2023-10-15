# My laboratory work #1
https://flask-rest-api-lab1.onrender.com
# flask-rest-api-lab1

Для запуску у себе на пк 

Потрібно клонувати проект в свою робочу директорію:
```
> git clone https://github.com/vetshem/flask-rest-api-lab1.git
```
Створити віртуальне середовище за допомогою venv:
```
> python3 -m venv env
```
Активувати віртуальне середовище:
```
> source ./env/bin/activate
```
Встановити flask допомогою команди:
```
> pip install flask
```
Тут є .flaskenv файл, тому потрібно поставити python-dotenv:
```
> pip install python-dotenv
```
Далі потрібно збілдити image такою командою:
```
>  docker build --build-arg PORT=<your port> . -t <image_name>:latest
```
Якщо image упішно збілдився, то його можна запустити і перевірити:
```
> docker run -it --rm --network=host -e PORT=<your port> <image_name>:latest
```
Збілдити контейнер: 
```
> docker-compose build
```
Запустити контейнер:
```
> docker-compose up
```
