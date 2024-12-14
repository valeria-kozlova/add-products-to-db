# Автоматизация тестирования системы управления товарами QualIT
## 📄 Описание
Проект предназначен для автоматизации тестирования веб-интерфейса системы управления товарами QualIT. Реализованы тесты для добавления новых товаров, проверки их корректного добавления в базу данных и предотвращения дублирования.

## 🛠 Технологии
- Java, JUnit 5
- Selenium WebDriver
- H2 Database (в памяти)
- Maven
## 📂 Структура проекта
- config/ — настройка базы данных
- utils/ — SQL-операции
- pages/ — классы Page Object
- tests/ — тестовые сценарии
## 🚀 Установка
1. Клонируйте проект:
```bash
git clone https://github.com/valeria-kozlova/add-products-to-db
```
2. Настройте chromedriver.
3. Запустите тесты через Maven или IDE.
## 🔌Подключение к стенду
1. Создайте папку Working Project на диске C.
2. Скачайте .jar файл по [ссылке](https://drive.google.com/file/d/18bI8rR9uPjVUNbSPIXBs84qViW0_VFpg/view).
3. Скопируйте скачанный файл в созданную папку.
4. Откройте консоль cmd.exe и переключитесь в папку с файлом командой:
```bash
cd C:\Working Project
```
5. Запустите стенд с помощью команды:
```bash
java -jar qualit-sandbox.jar
```
6. Перейдите по адресу: http://localhost:8080.
7. Для работы со стендом используйте вкладку "Песочница" - "Товары".
## 📊Параметры базы данных
1. После запуска стенда откройте консоль базы данных: http://localhost:8080/h2-console/
2. Укажите следующие параметры:
- БД: H2 Embedded
- URL: jdbc:h2:tcp://localhost:9092/mem:testdb
- Login: user
- Password: pass
## 🌟 Функционал
- Проверка добавления товаров.
- Тестирование дублирования записей.
- Интеграция с базой данных.
