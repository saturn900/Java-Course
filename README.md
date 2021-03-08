# Spring MVC

+ Реализовать и сконфигурировать сервисы в tracker-core и server-core.

    + 1 В практической работе «Введение в Spring» в модуле tracker-core был разработан Сервис отправки сообщений на центральный сервис по расписанию, который каждую минуту (периодичность – опция настройки) отправляет накопленные данные на центральный сервер в формате json. В предыдущей работе реальная отправка данных на Центральный сервер не осуществлялась. Требуется реализовать действительную отправку координат.

        + 1.1 Реорганизуйте tracker-core в виде приложения Spring Boot.

        + 1.2 Создайте компонент restTemplate.

        + 1.3 Используйте компонент restTemplate в сервисе отправки координат для выполнения POST запроса, в теле которого будут передаваться координаты по мере их поступления от сервиса GPS. Для выполнения POST-запроса подберите соответствующий метод в классе RestTemplate.

    + 2 В модуле server-core создайте веб-приложение с сервисом приема координат от tracker-core.

        + 2.1 Создайте приложение Spring Boot в server-core. 
          
        + 2.2 Добавьте контроллер для приема координат в виде POST запроса. Контроллер выводит полученные координаты в лог и в текстовый файл.

    + 3 Во всех приложениях использовать вывод в лог. Использование System.out запрещено.