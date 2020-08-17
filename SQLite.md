# Гайд по установке SQLite на Windows
1. Нужно зайти на сайт `sqlite`, на страницу загрузки: [https://www.sqlite.org/download.html](https://www.sqlite.org/download.html)
2. Перейти к разделу **Precompiled Binaries for Windows** и скачать файлы `sqlite-tools-win32 - *.zip` и `sqlite-dll-win32 - *.zip` (обведено на картинке)

![SQLite](https://raw.githubusercontent.com/EgorZak21/SQLite-Guide/master/img/sqlite.jpg)

3. Разархивировать `.zip` файлы , найти в разархивированных папках файлы `sqlite3.def`, `sqlite3.dll` и `sqlite3.exe` (они либо находятся сразу в архиве, либо внутри папки в архиве)
4. Создать папку `sqlite` на диске C `(C:\sqlite\)` и перенести туда эти 3 файла
5. Добавить эту папку `C:\sqlite\` в **PATH** - [Инструкция по добавлению в **PATH**](https://github.com/EgorZak21/SQLite-Guide/blob/master/PATH.md)
6. После добавления в **PATH** открываем (перезапускаем) `cmd` и пишем команду 
```bash
sqlite3 --version
```
Вывод будет примерно такой:

![SQLite](https://raw.githubusercontent.com/EgorZak21/SQLite-Guide/master/img/sqlite-check.jpg)
