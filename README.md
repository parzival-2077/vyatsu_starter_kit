# 🎓 Набор программ и приложений для легкого старта в ВятГУ
Небольшая помощь для первокурсников

## 🔍 Навигация
- [📝 Конспекты](#-конспекты)
- [💻 Программы](#-программы)
- [📊 Отчеты](#-отчеты)

---

## 📝 Конспекты

### Рекомендуемые инструменты
Конспекты можно вести в:
- Word
- Блокнот
- OneNote
- Google Docs

**Лучшая альтернатива** - [Obsidian](https://obsidian.md/download) (локальный аналог Notion)

### Примеры оформления
| С исходным кодом | Без кода |
|------------------|----------|
| <img width="500" src="https://github.com/user-attachments/assets/a4ff0c77-d8df-411b-898d-219b65d2892d"> | <img width="500" src="https://github.com/user-attachments/assets/d7a05833-5a2a-4faa-b1c0-2403333f55ea"> |

📌 [Пример конспекта](/18.03.2025.pdf)

> 💡 **Совет:** Самая удобная тема для Obsidian - "Simply Colorful"

---

## 💻 Программы

### 🔹 PascalABC.NET
[Скачать установщик](https://pascalabc.net/downloads/PascalABCNETSetup.exe)

### 🔹 Lazarus IDE
[Официальный сайт](https://www.lazarus-ide.org/) | 
[Установщик Win64](https://sourceforge.net/projects/lazarus/files/Lazarus%20Windows%2064%20bits/Lazarus%204.2/lazarus-4.2-fpc-3.2.2-win64.exe/download)

### 🔹 Настройка C/C++ в VSCode
Вот тут уже начинаются проблемы, поэтому небольшой гайд.
1. Скачиваем [Visual Studio Code](https://code.visualstudio.com/)
2. Скачиваем установщик [компилятора MSYS2](https://github.com/msys2/msys2-installer/releases/download/2024-12-08/msys2-x86_64-20241208.exe)
3. Запускаем установщик. Соглашаемся со всем, что есть
4. После установки прожимаем галочку "Run MSYS2 now" и завершаем установку.
5. Появится командная строка. В ней пишем(именно пишем, скопировать не получится) - `pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain`
6. Появится вот такая штука. Нажимаем enter <img width="1071" height="362" alt="image" src="https://github.com/user-attachments/assets/61a6896d-6fe6-400b-b69b-3a5f899ede29" />
7. Подтвержаем выбор Y(Yes)
8. Ждем
9. Добавим путь к компиляторам в PATH для удобного использования в терминале:
    - Откройте *Панель управления -> Система -> Дополнительные параметры -> Переменные среды* или введите в поиске *Переменные среды*
    - В переменную `Path` добавьте:
    ```ps
    C:\msys64\ucrt64\bin
    ```
    ![alt text](pics/environment-variables.png)

    - Проверяем установку в терминале:
    ```ps
    gcc -v
    ```
    Всё установилось если после ввода комманды выше вы получили примерно такой вывод:
    ![alt text](pics/gcc-check.png)
10. Запускаем VS Code
11. Выберите значок «Расширения» на панели активности или используйте сочетание клавиш ( Ctrl+Shift+X )
12. Ищем 'C/C++' от Microsoft
13. Выберите Установить
14. Создайте папку на диске С с любым названием на АНГЛИЙСКОМ языке
15. Укажите эту папку как основную для создания проектов в VS code

### 🔹 Arduino
[Скачать Arduino IDE](https://www.arduino.cc/en/software/) |
[Драйвер CH340](https://wiki.amperka.ru/_media/articles:driver-ch340:ch340ser-windows.zip) | [VSCode + PlatformIO IDE](https://platformio.org/platformio-ide) + [Расширение Serial Monitor](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-serial-monitor)

### 🔹 Microsoft Office
[Microsoft Office](https://cloud.mail.ru/public/zMaw/2ERQnvgHM) | [ONLYOFFICE](https://www.onlyoffice.com/download-desktop.aspx) | [Google Docs](https://docs.google.com/) (онлайн)

### 🔹 Logisim-evolution (Информатика 2 семестр)
[Logisim-evolution](https://github.com/logisim-evolution/logisim-evolution/releases/download/v3.9.0/logisim-evolution-3.9.0-x86_64.msi) (Построение и симуляция логических схем)

## 📊 Отчеты
### LaTeX редакторы
- Рекомендуем [Overleaf](https://ru.overleaf.com/) (онлайн-редактор)
- [LaTeX в VSCode + LaTeX Workshop](/VSCodeTeX.md) (оффлайн)
- [TeXstudio](https://www.texstudio.org/) (оффлайн)
- [MiKTeX](https://miktex.org/download) (оффлайн)

📄 [Пример отчета](https://www.overleaf.com/read/hwmjrjqbpygr#798ab1)

### Схемы алгоритмов 
Используйте [draw.io](https://github.com/jgraph/drawio-desktop/releases/tag/v28.0.6) | 
[Декстопная версия Windows](https://github.com/jgraph/drawio-desktop/releases/download/v28.0.6/draw.io-28.0.6-windows-installer.exe)

