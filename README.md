# Реализация аналога ArrayList

Это проект для реализации собственного аналога класса `ArrayList` в Java с использованием массивов. Цель проекта — помочь вам лучше понять, как работают коллекции в Java на низком уровне.

## Описание задания

Вам необходимо реализовать класс `DefaultCustomArrayList`, который будет соответствовать интерфейсу `CustomArrayList`. Данный интерфейс должен содержать следующие методы:

- `boolean add(E element)`: Добавляет элемент в конец списка.
- `boolean remove(E element)`: Удаляет первый встреченный элемент из списка. Возвращает `true`, если элемент был успешно удален.
- `E get(int index)`: Возвращает элемент по указанному индексу.
- `int size()`: Возвращает количество элементов в списке.
- `boolean isEmpty()`: Возвращает `true`, если список пуст.
- `void clear()`: Очищает список.
- `boolean contains(E element)`: Проверяет, содержится ли элемент в списке.
- Реализуйте интерфейс `Iterable<E>`, чтобы можно было использовать список в цикле `for-each`.

## Обобщения (Generics) в Java

### Что такое Generics?

Обобщения (или Generics) позволяют создавать классы, интерфейсы и методы с указанием параметров типов, что позволяет типу данных быть параметризованным. Это особенно полезно в коллекциях, так как предоставляет безопасность типов во время компиляции и устраняет необходимость приведения типов.

### Где они используются в этом проекте?

В вашем проекте вы должны использовать обобщения для создания `CustomArrayList<E>`, что позволяет использовать разные типы данных (например, Integer, String) с одной реализацией коллекции. Обобщение `<E>` обозначает тип элемента списка.

### Полезные ресурсы по Generics

1. **Официальная документация Java**:
   - [Generics в Java (оф. документация)](https://docs.oracle.com/javase/tutorial/extra/generics/)

2. **Дополнительные ресурсы**:
   - [Java Generics Tutorial на Baeldung](https://www.baeldung.com/java-generics) — подробное руководство с примерами.
   - [Generics в Java: подходы и методы](https://www.journaldev.com/1663/java-generics-example-method-class-interface) — пояснения на JournalDev с примерами использования.

## Получение проекта

1. **Клонирование репозитория**

   Склонируйте этот репозиторий на ваш локальный компьютер с помощью команды:

   ```bash
   git clone https://github.com/jegius/arrays-homework.git
   ```

2. **Переход в каталог проекта**

   Перейдите в директорию проекта:

   ```bash
   cd custom-arraylist
   ```

## Установка зависимостей

Перед запуском проекта и тестов необходимо установить зависимости.

1. **Использование Maven для установки зависимостей**

   Выполните команду:

   ```bash
   mvn clean install
   ```

   Эта команда соберет проект и загрузит все необходимые зависимости, указанные в файле `pom.xml`.

2. **Загрузка зависимостей в IDE**

   - **IntelliJ IDEA**
      - Откройте проект в IntelliJ IDEA.
      - Если проект открыт, но зависимости не подгружены, кликните правой кнопкой мыши по файлу `pom.xml` в дереве проекта и выберите `Maven -> Reload Project`.
      - Убедитесь, что в правой панели Maven все зависимости установлены без ошибок.

   - **Eclipse**
      - Откройте проект в Eclipse.
      - Щелкните правой кнопкой мыши по проекту и выберите `Maven -> Update Project`.
      - Убедитесь, что все зависимости подгружены корректно.

## Запуск тестов

Для того чтобы убедиться в правильности реализации методов, выполните следующие шаги:

1. **Запуск тестов с помощью Maven**

   Используйте следующую команду Maven для запуска тестов:

   ```bash
   mvn test
   ```

   Эта команда соберет проект и выполнит все тесты, находящиеся в директории `src/test/java`.

## Структура проекта

- `src/main/java`: Содержит интерфейс и класс для реализации `CustomArrayList`.
- `src/test/java`: Содержит модульные тесты для вашей реализации.

## Советы по выполнению задания

- Убедитесь, что все методы реализованы согласно спецификации интерфейса.
- Проверьте корректность обработки индексов и используйте исключения при необходимости.
- Обратите внимание на оптимизацию работы с массивами — увеличение их размера, копирование и удаление элементов.

## Проверка результата

После завершения задания и успешного прохождения всех тестов, ваш проект должен корректно работать как аналог `ArrayList`, поддерживая основные операции с коллекциями.

Удачи в выполнении задания и успешного кодирования!
