# Kinopoisk Project

Этот проект был создан с помощью [Angular CLI](https://github.com/angular/angular-cli) версии 17.3.4.

## Development server

Запустите `ng serve` для сервера разработки. Перейдите по адресу 'http://localhost:4200/'. Приложение автоматически перезагрузится, если вы измените какой-либо исходный файл.

## Code scaffolding

Запустите `ng generate component component-name` чтобы сгенерировать новый компонент. Вы также можете использовать `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build
Запустите `ng build` чтобы собрать проект. Артефакты сборки будут храниться в каталоге `dist/` directory.

## Running unit tests

Запустите `ng test`, чтобы выполнить модульные тесты через [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Запустите `ng e2e` чтобы выполнить сквозные тесты на выбранной вами платформе. Чтобы использовать эту команду, вам необходимо сначала добавить пакет, реализующий возможности сквозного тестирования.

## Further help

Чтобы получить дополнительную помощь по Angular CLI, используйте `ng help` или посетите страницу [Angular CLI Overview and Command Reference](https://angular.io/cli).



## Инструкция: 

### Версии пакетов и ангуляра

Package Manager: npm 10.2.4

OS: win32 x 64

Angular: 17.3.4

@angular-devkit/architect           0.1703.4@angular-devkit/build-angular        17.3.4

@angular-devkit/core            17.3.4@angular-devkit/schematics      17.3.4

@schematics/angular             17.3.4rxjs                            7.8.1

typescript                      5.4.5zone.js                         0.14.4



1. Установите последнюю версию ангуляр

2. Скопируйте этот репозиторий в свою локальную папку гит

3. Установите все необходимые пакеты
 
4. В терминале перейдите к расположению проекта и запустите через ng serve




## Процесс:

1. Было использовано две API ссылки т.к один не выдавал список фильмов, а в другом была недостаточность информации. Их вы можете посмотреть в папке movie.service.ts

2. Были использованы методы *ngFor *ngIf  для более чистого кодинга и понятных условии

3. Routing был применен для перемещения между компонентами
   
/movies: Общий список фильмов

/movies/:title: Детали о выбранном фильме

/my-movies: список избранных фильмов

4. Есть функция пополнения списка приемом нажатия на кнопку "Load more..." в конце списка. каждый раз добавялющая 20 фильмов к существующему списку.

5. Поисковая система по названию фильма. Если нет совпадении по поиску то выводится оповещающий текст на странице. Если вы ввели пустую строку то выведет полный список.

6. Также можно добавить в список избранных и так же удалить из этого списка. Если список пуст то выводится ответное сообщение и кнопка перекидыващая на главную страницу

7. Нажатием на ссылку Learn more.. на любом из элементов списка вы переходите на страницу с более подробными деталями о фильме.



## Компромиссы, ошибки:

1. Было сложно работать с двумя API ссылками одновременно, их нужно было синхронизировать и много других нюансов. Однако это было нужно так как нужен был список для поиска из api.themoviedb.org . Но и без данных о жанрах c omdapi.com не обошлось бы. Поиск нужного апи заняло долгое время.

2. Вместо пагинации с номерами страниц я сделала кнопку просто дополняющую список. 

3. Некоторые фильмы которые есть в themoviedb нету в omdapi. И так как с первого я беру общий список а со второго детальные данные иногда могут встретиться фильмы с пустыми полями для информации. Если бы было время не поджимало я бы смогла сделать компонент/сообщение которое выводится когда данных о фильме нету.

4. Иногда при поиске выводится по несколько одинаковых элементов. Думаю это из за того что расширение списка нужно доработать.

