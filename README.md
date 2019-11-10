---
title: Сервис
---

# Описание

Лэндфист предоставляет доступ к повторным ландшафтным фотоснимкам, которые были сделаны с одной и той же точки съёмки в разное время. Повторные фотоснимки позволяют оценить динамику изображаемых растительных сообществ, которую связывают с климатическими изменениями, фиксируемыми за последние десятилетия, в том числе и на территории Урала.

![Количество повторных снимков в сервисе](https://img.shields.io/endpoint?url=https://landphist.azurewebsites.net/api/stat/shields/photos&amp;style=for-the-badge&amp;label=Снимков)

Таганай. Митькины скалы
![Таганай. Митькины скалы](https://uraloved.ru/images/news/ekb/les-podn-v-gori-3.jpg)

Таганай. Двуглавая сопка
![Таганай. Двуглавая сопка](https://uraloved.ru/images/news/ekb/les-podn-v-gori-2.jpg)

# Установка

Для просмотра фотоснимков необходимо установить приложение `Sas.Планета` и добавить слой фотографий `Лэндфист`. `Sas.Планета` работает только под операционной системой `Windows`. По приведенным в верхней части страницы ссылкам, последовательно скачайте и установите приложение и архив со слоем фотографий.

Если приложение еще не было установлено, установите его в систему, например, в папку `...\Sas.Planet`.

Слой снимков должен быть установлен в папку с картами приложения `...\Sas.Planet\Maps\sas.maps\`. Извлеките папку `Lps` из архива в указанную папку с заменой файлов.

Для дальнейшей работы приложение необходимо перезапустить.

В запущенном приложении `Sas.Планета` нажмите на кнопку `Выбор слоев, отображаемых поверх основной карты` и в раскрывающейся группе `Лэндфист` выберите необходимые для отображения слои.

# Обратная связь

Чтобы сообщить нам о проблеме, заведите [ишью](https://github.com/PavelQuash/Landphist/issues) на GitHub.

# Api

`/api/geo/box?minLatitude=...&maxLatitude=...&minLongitude=...&maxLongitude=...` - получение точек в формате `kml` в указанной области

`/api/photos/{photoId}/info` - информация о снимке

`/api/photos/{photoId}/size/{sizeAlias}` - скачать снимок
