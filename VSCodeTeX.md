# 📖 Гайд по установке и настройке LaTeX в VSCode на Windows 10/11

Мы будем использовать:

* **TeX Live** (дистрибутив LaTeX)
* **Visual Studio Code**
* Расширения **LaTeX Workshop** и **LaTeX Utilities** для **Visual Studio Code**

## 1. Установка TeX Live

1. Скачайте установщик TeX Live:
  👉 [https://tug.org/texlive/acquire-netinstall.html](https://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe)

2. Запустите `install-tl-windows.exe`.

* По умолчанию ставится в `C:\texlive\2025`.
* Можно оставить стандартные настройки.

3. После установки **добавьте TeX Live в PATH**:

* Откройте *Панель управления → Система → Дополнительные параметры → Переменные среды*.
* В переменную `Path` добавьте:

     ```ps
     C:\texlive\2025\bin\windows
     ```

1. Проверьте, что всё работает:
   Откройте PowerShell и введите:

   ```ps
   pdflatex --version
   ```

   Если выводится версия — всё установлено.

## 2. Установка Visual Studio Code

1. Скачайте VSCode:
   👉 [https://code.visualstudio.com/download](https://code.visualstudio.com/download)

2. Установите с галочкой «Добавить в PATH» (удобно для терминала).

## 3. Установка расширений

Откройте VSCode и установите расширения (через `Ctrl+Shift+X`):

* **LaTeX Workshop** (основное расширение для компиляции, просмотра PDF)
* **LaTeX Utilities** (подсказки, команды, автодополнение цитат и окружений)

## 4. Настройка LaTeX Workshop

Откройте настройки (`Ctrl+,` → поиск `latex-workshop`).

### Минимальные настройки в `settings.json`

Откройте `Ctrl+Shift+P → Preferences: Open User Settings (JSON)` и вставьте:

```json
{
    "latex-workshop.latex.tools": [
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "%DOC%"
            ]
        }
    ],

    "latex-workshop.latex.recipes": [
        {
            "name": "latexmk 🔄",
            "tools": ["latexmk"]
        }
    ],

    "latex-workshop.view.pdf.viewer": "tab", 
    "latex-workshop.synctex.afterBuild.enabled": true,
    "latex-workshop.message.update.show": false
}
```

### Что это даёт

* `latexmk` автоматически собирает `.tex` в `.pdf`.
* Просмотр PDF прямо в VSCode (во вкладке).
* Поддержка **SyncTeX** — можно кликать в PDF и переходить к строке в `.tex`.

---

## 5. Проверка работы

1. Создайте папку, откройте её в VSCode.
2. Создайте файл `main.tex`:

```latex
\documentclass{article}
\begin{document}
Hello, \LaTeX!
\end{document}
```

3. Нажмите `Ctrl+Alt+B` (команда **Build LaTeX project**).
4. В правой части VSCode откроется PDF с результатом.

---

## 6. Дополнительно

* **LaTeX Utilities**: добавляет умные сниппеты (`\begin{...}` автодополняется).
* Если используете BibTeX для библиографии, то LaTeX Workshop автоматически подхватит `.bib` файлы.
* Можно поменять PDF-просмотрщик на внешний (`SumatraPDF`), если нужен более быстрый просмотр.

---

Таким образом, у тебя получается полноценная среда:
VSCode + TeX Live + LaTeX Workshop + LaTeX Utilities = готовый LaTeX-IDE 🚀

---

Хочешь, я добавлю ещё раздел про настройку **SumatraPDF** как внешнего просмотрщика с поддержкой прямого перехода строка↔PDF (очень удобно), или оставим только встроенный?
