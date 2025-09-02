# 📖 Гайд по установке и настройке LaTeX в VSCode на Windows 10/11

Мы будем использовать:

- 🖋 **TeX Live** — дистрибутив LaTeX  
- 🖥 **Visual Studio Code** — удобный текстовый редактор  
- ⚙️ Расширения **LaTeX Workshop** и **LaTeX Utilities** для **Visual Studio Code**

---

## 1️⃣ Установка TeX Live

1. 🔗 Скачайте установщик TeX Live:  
   [install-tl-windows.exe](https://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe)

2. 🚀 Запустите `install-tl-windows.exe`.

   - По умолчанию ставится в `C:\texlive\2025`  
   - Можно оставить стандартные настройки  
   - Установка займет какое-то время...

3. 🛠 После установки **добавьте TeX Live в PATH**:

   - Откройте *Панель управления → Система → Дополнительные параметры → Переменные среды*  
     или введите в поиске *Переменные среды*  

   - В переменную `Path` добавьте:

     ```powershell
     C:\texlive\2025\bin\windows
     ```

   ![Настройка переменных среды](pics/environment-variables.png)

4. ✅ Проверьте, что всё работает:  
   Откройте PowerShell и введите:

   ```powershell
   pdflatex --version
   ```

Если выводится версия — всё установлено.

---

## 2️⃣ Установка Visual Studio Code

1. 🔗 Скачайте VSCode:
   [https://code.visualstudio.com/download](https://code.visualstudio.com/download)

2. 🖱 Установите с галочкой **«Добавить в PATH»** (удобно для терминала).

---

## 3️⃣ Установка расширений

Откройте VSCode и установите расширения:

* 📦 **LaTeX Workshop** — основное расширение для компиляции и просмотра PDF
* 🧰 **LaTeX Utilities** — подсказки, команды, автодополнение цитат и окружений

---

## 4️⃣ Проверка работы

1. 📁 Создайте папку и откройте её в VSCode.

2. 📝 Создайте файл `main.tex`:

   ```latex
   \documentclass{article}
   \begin{document}
   Hello, \LaTeX!
   \end{document}
   ```

3. ⚡ Нажмите `Ctrl+Alt+B` (команда **Build LaTeX project**)

4. 🖼 В правой части VSCode откроется PDF с результатом.