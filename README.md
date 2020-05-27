# Задание на дипломный проект «“Облачный архиватор» 1 блока «Основы языка программирования Python».

Облачные хранилища стали для человека уже нормой. Загрузить альбом с фотографиями или поделиться какими-либо документами. Но есть одна проблема, там может закончиться место. Было бы неплохо уметь архивировать самый тяжелый файла или папку и загружать её обратно в облако. Так мы можем сохранить больше свободного места на облаке. В качестве облака будем использовать Яндекс.Диск.
Токен можно получить на странице [Полигона Яндекс.Диска](https://yandex.ru/dev/disk/poligon/)

## Задание:
Нужно найти на Диске самый тяжелый файл/папку(решает пользователь), заархивировать его на компьютере. И загрузить архив обратно на Диск.

### Входные данные: 
Программа запрашивает токен для работы с API Яндекс.Диска.

### Выходные данные: 
Вывести в json-файл информацию о заархивированном файле
```javascript
    {
    “file_name”: “diplom.docx”, 
    “size”: “идентификатор группы”, 
    “path”: “disk:/Netology/diplom.docx”
    }
```

### Требования к программе:
1. Использовать REST API Я.Диска и ключ, полученный с полигона
2. Для архивации файлов или папки использовать библиотеку zipfile
3. Предлагать опционально пользователю удалить с Диска файл/папку вместо загружаемого файла.
4. Сделать прогресс-бар для отслеживания процесса программы.
5. Код программы удовлетворяет PEP8.

### Дополнительные требования (не обязательны для получения диплома):
1. найти топ 10 файлов по размеру
2. записать в гугл таблицу список этих файлов в табличном виде - название каталог хранения, размер.