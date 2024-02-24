# LolCat

> Реализация lolcat на Си


## Table of Contents

* [Introduction](#Introduction)
* [Flags](#Flags)
* [Build](#build)
* [Install](#Install)
* [Uninstall](#Uninstall)

## Introduction


https://github.com/BulatRuslanovich/LolCat/assets/113189826/44a0f9b6-b092-4cd5-9b4c-4f07e18e4385
> Установка производится в домашнюю папку $HOME/.
## Введение

`LolCat` — это захватывающий инструмент, который призван придать вашему терминалу красочную радужную атмосферу. Представьте себе мир, где вывод текста становится ярким и привлекательным, словно каждая буква оживает в цветной вспышке. Это именно то, что предлагает `LolCat`.

## Очарование цветами

С помощью `LolCat` вы сможете не только конкатенировать содержимое файлов или стандартного ввода, но и добавить им приятную гамму. Благодаря встроенным возможностям каждый вывод станет неповторимым произведением искусства.

## Гибкость и контроль

`LolCat` предлагает широкий набор флагов для настройки вывода. Вы можете легко настроить частоту радуги, управлять цветовыми градиентами, добавить случайные цвета или даже инвертировать передний и задний план. Это дает вам полный контроль над тем, как ваш текст будет представлен.

## Простота использования

Несмотря на свои многочисленные возможности, `LolCat` остается простым и интуитивно понятным инструментом. С легкостью устанавливайте и используйте его, чтобы добавить жизнь в ваш терминал.

## Flags
- `--horizontal-frequency <d>`, `-h <d>`: Устанавливает горизонтальную частоту радуги (по умолчанию: 0.23).
- `--vertical-frequency <d>`, `-v <d>`: Устанавливает вертикальную частоту радуги (по умолчанию: 0.1).
- `--force-color`, `-f`: Принудительно использует цвет даже если стандартный вывод не является терминалом.
- `--no-force-locale`, `-l`: Использует кодировку из системной локали вместо предполагаемой UTF-8.
- `--random`, `-r`: Включает случайные цвета.
- `--seed <d>`, `-s <d>`: Устанавливает случайные цвета на основе заданного seed, подразумевает использование флага `--random`.
- `--color_offset <d>`, `-o <d>`: Начинает с другого цвета.
- `--gradient <g>`, `-g <g>`: Использует градиент цвета от указанного начального до конечного цвета, формат: `-g ff4444:00ffff`.
- `--24bit`, `-b`: Выводит в 24-битном "настоящем" RGB-режиме (медленнее и не поддерживается всеми терминалами).
- `--16color`, `-x`: Выводит в 16-цветном режиме для базовых терминалов.
- `--invert`, `-i`: Инвертирует передний и задний план.

## Добавление LolCat/bin в переменную среды PATH

1. Откройте терминал.
2. Отредактируйте файл `~/.bashrc`, который является скриптом оболочки для bash, используемый при входе в систему. Для этого выполните команду:
    ```bash
    vim ~/.bashrc
    ```
   Вы можете использовать любой текстовый редактор вместо `vim`, если предпочитаете.
3. Прокрутите файл до конца и добавьте следующую строку:

    ```bash
    export PATH=$PATH:~/LolCat/bin
    ```
4. Сохраните изменения и закройте редактор.

5. Обновите текущую оболочку, чтобы изменения вступили в силу, выполнив следующую команду:

    ```bash
    source ~/.bashrc
    ```

Теперь папка `LolCat/bin` добавлена в вашу переменную среды `PATH` и все исполняемые файлы из этой папки, включая `lolcat`, будут доступны для запуска из любого места в вашей оболочке.
> Для ~/.zshrc проделываем все тоже самое, только заменяя ~/.bashrc на ~/.zshrc


## Build
```bash
git clone git@github.com:BulatRuslanovich/LolCat.git
cd LolCat/src
make
```

## Install
```bash
git clone git@github.com:BulatRuslanovich/LolCat.git
cd LolCat/src
make install
```

## Uninstall
```bash
cd LolCat/src
make uninstall
```
