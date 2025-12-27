
 ```bash
 # установка глобального пользователя Git (для всех проектов)
git config --global user.name "Pragmatic Programmer"

# установка глобального email пользователя Git (для всех проектов)
git config --global user.email "prag_prog@gmail.com"

# включение цветного вывода информации (в ряде случаев включено по умолчанию)
git config --global color.ui true

# вывод списка настроек
git config --list

# вывод имени пользователя/email из настроек
git config user.name
git config user.email

# вывод истории команд
history

# установка локальной настройки Git (для конкретного репозитория)
git config user.name "Pragmatic Programmer"
git config user.email "prag_prog@gmail.com"

 ```

### Расположение конфиг-файла

**1. Системные настройки Git (для всех пользователей)**

- C:\Program Files\Git\etc\gitconfig

 **2. Глобальные настройки (для текущего пользователя)**

- %USERPROFILE%\.gitconfig

**3. Локальные настройки (для конкретного репозитория)**

- <Путь_к_репозиторию>\.git\config

### Часто используемые команды
```bash
# посмотреть состояние файлов в индексе
git status

# посмотреть историю коммитов
git log

# вывести на экран содержимое указанного файла
cat page1.html

# добавить в индекс указанный файл
git add page1.html

# сделать коммит (требует ввода текстового сообщения)
git commit

```

### Полезные команды для настройки окружения
```bash
# вывод списка настроек
git config list

# установить редактор по умолчанию для Git
git config core.editor nano

# добавить в индекс все файлы в текущей папке
git add .

# добавить в индекс указанный файл
git add page1.html

# посмотреть историю коммитов в компактном виде
git log --oneline
```
