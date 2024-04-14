# Kinopoisk Project

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.3.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.


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


