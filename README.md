## Дата выполнения

3.09.2024

# Currency Converter SPA

Currency Converter SPA — это веб-приложение для конвертирования валют. Приложение разработано с использованием Vue.js и поддерживает конвертацию валют USD, EUR и RUB. Пользователь может выбрать основную валюту сайта, а также произвести конвертацию между двумя валютами с точностью до двух знаков после запятой.

## Требования

Перед установкой и запуском убедитесь, что у вас установлены следующие инструменты:

- Node.js (версия 14 или выше)
- npm (версия 6 или выше) или yarn

## Установка

1. Перейдите в директорию проекта:

    ```bash
    cd currency-converter-spa
    ```

2. Установите зависимости:

    С использованием npm:

    ```bash
    npm install
    ```

    С использованием yarn:

    ```bash
    yarn install
    ```

## Запуск

Для разработки:

1. Запустите сервер разработки:

    ```bash
    npm run dev
    ```

    или

    ```bash
    yarn dev
    ```

    Приложение будет доступно по адресу http://localhost:3000.

2. Для сборки и запуска в production:

    Создайте сборку приложения:

    ```bash
    npm run build
    ```

    или

    ```bash
    yarn build
    ```

3. После успешной сборки запустите приложение:

    ```bash
    npm start
    ```

    или

    ```bash
    yarn start
    ```

## Задание

Написать SPA для конвертирования валют. В приложении должен быть хедер и 2 страницы:

### Хедер:
- Ссылки на 2 страницы: "Главная" (/) и "Конвертация" (/convert).
- Dropdown с выбором основной валюты сайта.

### Главная страница:
- Отображение курсов валют по отношению к основной валюте сайта.
- Пример: если основная валюта RUB, то пользователь видит, что 1 USD = 91.45 RUB, 1 EUR = 101.74 RUB.

### Страница конвертации:
- Форма, состоящая из 2 строк.
- В каждой строке должен быть Dropdown с выбором валюты и числовой Input.
- В каждом Dropdown должна быть выбрана одна из валют по умолчанию.
- При изменении значения в любом из двух Input автоматом конвертировать и изменять значение в другом Input.
- Все значения при конвертации округлять до 2 знаков.

### Примечание:
- Курсы валют можно получать с этого API: [GET https://status.neuralgeneration.com/api/currency](https://status.neuralgeneration.com/api/currency) или использовать любое открытое API.
- Для реализации использовать фреймворк Vue3 и любые библиотеки, которые считаете нужными.
- Поддержка 3 валют: USD, EUR, RUB.
- Приветствуется разделение на компоненты и налаживание хороших связей между ними.
- Плюсом будет добавление проверок в Input и отображение ошибок, например, при вводе текстовых значений.