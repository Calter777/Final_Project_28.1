# Final_Project_28.1
Заказчик передал вам следующее задание:

1. Протестировать требования.

2. Разработать тест-кейсы (не менее 15). Необходимо применить несколько техник тест-дизайна.

3. Провести автоматизированное тестирование продукта (не менее 15 автотестов). Заказчик ожидает по одному автотесту на каждый написанный тест-кейс. Оформите свой набор автотестов в GitHub.

4. Оформить описание обнаруженных дефектов. Во время обучения вы работали с разными сервисами и шаблонами, используйте их для оформления тест-кейсов и обнаруженных дефектов. Если дефекты не обнаружены, то подумайте и опишите 3 потенциально возможных дефекта на данном ресурсе.

Приложите ссылку на документ с тест-кейсами, ссылку на GitHub с автотестами, ссылки на баги или документ с описанием этих багов.
→ Требования по проекту (.doc) 

→ Объект тестирования: https://b2c.passport.rt.ru 




В проект использовались: PageObject, Selenium и PyTest.

В корневой папке находятся файлы chromedriver.exe для запуска тестов с браузером google chrome, requirements.txt для установки необходимых для тестирования библиотек, settings.py с тестовыми данными.

Папка tests содержит файл для запуска автотестов: test

Папка pages содержит следующие файлы: base_page.py - базовая страница, от которой унаследованы все остальные классы, auth_page.py - содержит класс для страницы авторизация, registr_page.py - содержит класс для страницы регистрация 
locators.py - список локаторов на веб страницах, 

Для запуска тестов необходимо установить библиотеки командой:
- pip install -r requirements.txt

Запуск тестов при помощи команд в консоли:

- python -m pytest -v --driver Chrome --driver-path chromedriver.exe tests/test.py

Ссылка на тест кейсы: https://docs.google.com/spreadsheets/d/1_Ijgn-lrIk70E9vSyNRXjH20IRuU19qvDXzVrQU0c-M/edit?usp=sharing

P.S.Отдельные тесты могут "падать" из-за необходимости ввода каптчи .
