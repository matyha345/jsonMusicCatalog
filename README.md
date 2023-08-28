<h1 align="center">Данная структура позволит вам создавать фейковый RESTful API, обходя ограничение на количество запросов (ограничение в 500 запросов) с веб-сайта. <a href="https://rapidapi.com/apidojo/api/shazam" target="_blank">RapidAPI</a> </h1>


# <h3 align="center">В файле db.json содержатся данные для обработки запросов музыкальных композиций.</h3>

Команда  <h1>json-server db.json -p 4200</h1> используется для запуска локального сервера API с использованием инструмента json-server. Этот инструмент позволяет вам быстро создать фейковый RESTful API, используя данные из файла JSON (db.json). Ваше приложение может отправлять запросы к этому локальному серверу для имитации взаимодействия с настоящим удаленным сервером.

#
Давайте рассмотрим каждую часть команды:

json-server: Это команда, которая запускает инструмент json-server.

db.json: Это файл, содержащий данные в формате JSON. Эти данные будут предоставляться как эмулированный API сервером.

-p 4200: Этот флаг указывает на порт, на котором будет работать локальный сервер. В данном случае, сервер будет доступен по адресу http://localhost:4200.
#
Когда вы запустите эту команду, вы создадите локальный сервер, который будет слушать указанный порт и предоставлять данные из файла db.json по маршрутам, соответствующим структуре данных в файле. Например, если в db.json есть массив объектов, представляющих сущности tracks и properties, то вы можете получить список пользователей, отправив GET-запрос на  

* http://localhost:4200/properties

* http://localhost:4200/tracks.

Это полезный способ для разработчиков тестировать взаимодействие между фронтендом (например, веб-приложением) и бэкендом (API) в локальной среде без необходимости настройки настоящего сервера.

<div  display= "flex"
  align-items="center" >
 <img src="./image/json.png" alt="Alt img" width="250" height="auto">
 <img src="./image/handler.png" alt="Alt img" width="250" height="auto">
 <img src="./image/Request1.png" alt="Alt img" width="250" height="auto">
 <img src="./image/app.png" alt="Alt img" width="250" height="auto">
</div>
