[![Test Pelles C](https://github.com/Serge3leo/test-pellesc/actions/workflows/test-pellesc.yml/badge.svg)](https://github.com/Serge3leo/test-pellesc/actions/workflows/test-pellesc.yml)

# test-pellesc
Простая проверка установки Pelles C.

Репозиторий Chocolatey Software, Inc. содержит версии только до `12.0.2`,
версия `13.01-git-lfs` устанавливается из текущего репозитория GitHub (13.01,
23 Дек 2025 [https://www.pellesc.se](https://www.pellesc.se).

Похоже в версии `11.0.2` команда `cc` не работает на Windows 2022/2025.

# Проверка ошибки длинных имён
Команда `cc` имеет ошибку, в случае если она вызывается с явным указанием пути,
который имеет пробелы.

Проверяется два варианта её обхода в версиях 12.x и 13.x:
1. Установка в Pelles C в каталог без пробелов на пути. Задаётся параметром
   `install-workaround: true`;

2. Настройка переменных окружения как Short File Name (SFN). Задаётся
   параметром `env-workaround: true`;

# Использование
Сделать fork репозитория. Создать PR с префиксом имени `Test...`, в котором
можно изменить параметры `install-workaround` или `env-workaround`. Проверить
протокол GitHub Actions.

# Участие
Замечания (issues), добавления или исправления (pr) - принимаются и
приветствуются.

# Лицензия
[BSD-2-Clause © 2025 Сергей Леонтьев (leo@sai.msu.ru).](LICENSE)
