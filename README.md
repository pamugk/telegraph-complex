# Программный комплекс "Телеграф"

## О комплексе

Программный комплекс задумывался как реализация исключительно в самообразовательных целях подобия известного мессенджера Telegram с использованием лишь языка программирования "C".  
Ну и, в принципе, получилось вполне неплохо. Понятное дело, всей функциональности Telegram пока нет, но обмен сообщениями уже работает).  
Дальнейшая доработка вполне возможна.

## Состав комплекса

Комплекс состоит из двух основных компонентов: [серверной части](https://github.com/pamugk/telegraph-server "Репозиторий серверной части") и клиентской части.  
Сервер обрабатывает запросы клиентов и обеспечивает взаимодействие с хранилищем данных (для хранения данных используется БД PostgreSQL).  
Клиентская часть как таковая реализована [тут](https://github.com/pamugk/telegraph-client "Репозиторий клиентской части"). Она представляет собой переносимую библиотеку (в идеале, пока это просто куча кода), с использованием которой уже можно реализовывать клиентские приложения (как консольных, так и с графическим интерфейсом) за счёт использования уже реализованой функциональности и структур данных.  
Так, например, с использованием *почти* библиотеки клиентской части разработано [клиентское приложение](https://github.com/pamugk/gtk-telegraph "Репозиторий клиентского приложения") с использованием GTK - фреймворка для разработки кроссплатформенных (почти) приложений с графическим интерфейсом.
