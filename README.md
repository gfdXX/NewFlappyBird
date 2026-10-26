# Flappy Bird на JavaFX

![Java](https://img.shields.io/badge/Java-17-007396?logo=openjdk&logoColor=white)
![JavaFX](https://img.shields.io/badge/JavaFX-FXML-orange)
![Maven](https://img.shields.io/badge/Maven-build-C71A36?logo=apachemaven&logoColor=white)

Клон Flappy Bird — учебный проект по курсу Java, МГТУ им. Н.Э. Баумана, ИУ1 (весна 2022).
Птица — прямоугольник, который падает с ускорением и подпрыгивает по **пробелу**. Нужно пролетать между препятствиями: за каждое пройденное очко счёт растёт, при столкновении игра начинается заново.

## Устройство

| Класс | Роль |
|---|---|
| `Application` | запуск окна JavaFX и загрузка `view.fxml` |
| `Controller` | игровой цикл на `AnimationTimer`: гравитация, прыжок, генерация препятствий каждые 300 кадров, подсчёт очков, перезапуск |
| `Bird` | движение птицы по вертикали, прыжок, проверка гибели |
| `ObstaclesHandler` | создание пар препятствий со случайным просветом и их сдвиг влево |
| `CollisionHandler` | проверка пересечения прямоугольников |

## Как запустить

Нужны JDK 17+ и Maven:

```bash
mvn clean javafx:run
```

Или откройте проект в IntelliJ IDEA и запустите `Application`.

## Авторы

Салженикин Даниил и Галиев Эльдор ([eldor-galiev](https://github.com/eldor-galiev)), МГТУ им. Н.Э. Баумана.
