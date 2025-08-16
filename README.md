# Набор программ и приложений для легкого старта обучения в ВятГУ
Небольшая помощь для первокурсников

## Навигация 
1. [Конспекты](#1.-Конспекты)
2. Программы
3. [Отчеты](#3.-Отчеты)

## 1. Конспекты 
Конспекты можно вести в любой программе: Word, Блокнот, Notion(ушел из России) и тд. Все эти файлы могу быть разбросаны по системе и затруднять поиск нужных записей. Однако лучшей альтернативой для всего этого является - **[Obsidian](https://obsidian.md/download)**

#### Примеры основного оформления 
С исходным кодом 
<img width="1090" height="989" alt="image" src="https://github.com/user-attachments/assets/a4ff0c77-d8df-411b-898d-219b65d2892d" />

И как без него 
<img width="1086" height="1255" alt="image" src="https://github.com/user-attachments/assets/d7a05833-5a2a-4faa-b1c0-2403333f55ea" />

Пример конспекта - [тык](/18.03.2025.pdf)

> [!TIP]
> Самая удобная тема для Obsidian называется Simply Colorful

## 2 Программы 
Не так уж и много программ понадобится на 1 курсе, однако удобнее когда все они находятся в одном месте)

Pascal(ссылка на установщик) - [тык](https://pascalabc.net/downloads/PascalABCNETSetup.exe)

Lazarus(официальный сайт с сcылками на SourceForge)- [тык](https://www.lazarus-ide.org/index.php?page=downloads), [ссылка на установщик Win64](https://sourceforge.net/projects/lazarus/files/Lazarus%20Windows%2064%20bits/Lazarus%204.2/lazarus-4.2-fpc-3.2.2-win64.exe/download)

C - Вот тут уже начинаются проблемы, поэтому небольшой гайд.
1. Скачиваем Visual Studio Code - [тык](https://code.visualstudio.com/)
2. Скачиваем установщик компилятора для C [прямая ссылка](https://github.com/msys2/msys2-installer/releases/download/2024-12-08/msys2-x86_64-20241208.exe)
3. Запускаем установщик. Соглащаемся со всем, что есть
4. После установки нажимаем Run MSYS2 now
5. Появится командная строка. В ней пишем(именно пишем, скопировать не получится) - `pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain`
6. Появится вот такая штука. Нажимаем enter <img width="1071" height="362" alt="image" src="https://github.com/user-attachments/assets/61a6896d-6fe6-400b-b69b-3a5f899ede29" />
7. Подтвержаем выбор Y(Yes)
8. Ждем
9. Запускаем VS Code
10. Выберите значок «Расширения» на панели активности или используйте сочетание клавиш ( Ctrl+Shift+X ).
11. Ищем 'C' от Microsoft.
12. Выберите Установить
13. Создайте папку на диске С с любым названием на АНГЛИСКОМ языке.
14. Укажите эту папку как основную для создания проектов в VS code

Arduino - [ссылка на загрузку Win64](https://downloads.arduino.cc/arduino-ide/arduino-ide_2.3.6_Windows_64bit.exe), [ссылка на страницу загрузки](https://www.arduino.cc/en/software/)

Драйвер для Arduino Uno - [тык](https://wiki.amperka.ru/_media/articles:driver-ch340:ch340ser-windows.zip)

Если вам нужен Microsoft Office - [ссылка на облако](https://cloud.mail.ru/public/zMaw/2ERQnvgHM)

## 3. Отчеты
Отчеты пишутся в LaTeX. Обычно используем[Overleaf](https://ru.overleaf.com/)

> [!CAUTION]
> Пример отчета не редактируем. Открыли, посмотрели, скопировали, закрыли. НИЧЕГО НЕ УДАЛЯЕМ

Пример отчета в LaTeX - [тык](https://www.overleaf.com/8434914313vfywjqctbsks#9d8da1)

#### Схемы алгоритмов 
Проще всего создавать в [draw.io](https://github.com/jgraph/drawio-desktop/releases/tag/v28.0.6), [ссылка на загрузку Win64](https://github.com/jgraph/drawio-desktop/releases/download/v28.0.6/draw.io-28.0.6-windows-installer.exe)
