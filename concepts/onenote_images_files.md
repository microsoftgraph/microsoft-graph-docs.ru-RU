
# <a name="add-images-videos-and-files-to-onenote-pages"></a>Добавление изображений, видео и файлов на страницы OneNote

*__Относится к:__ пользовательские записные книжки в OneDrive | корпоративные записные книжки в Office 365*

С помощью элементов **img**, **object** и **iframe** вы можете добавлять изображения, видео и файлы на страницу OneNote при ее [создании](onenote-create-page.md) или [обновлении](onenote_update_page.md). 

- Элемент **img** используется для отрисовки изображения на странице.
- Элемент **iframe** используется для внедрения видео в страницу.
- Элемент **object** используется для добавления вложенного файла на страницу.


<a name="images"></a>
## <a name="adding-images"></a>Добавление изображений

Изображения можно добавлять по URL-адресу или путем отправки необработанных данных. Microsoft Graph поддерживает перечисленные ниже способы добавления изображений, логотипов и фотографий на страницы OneNote. 

[Добавление общедоступного изображения из Интернета](#add-a-public-image-from-the-web)  
Используйте элемент `img` с параметром `src="http://image-url"` и укажите URL-адрес общедоступного изображения. Отрисовывает изображение на странице OneNote.</p>
[Добавление изображения с помощью двоичных данных](#add-an-image-using-binary-data)</p>
Используйте элемент `img` с параметром `src="name:image-block-name"` и отправьте файл изображения в части данных составного запроса. Отрисовывает изображение на странице OneNote.</p>
[Добавление моментального снимка веб-страницы](#add-a-webpage-snapshot)</p>
Используйте элемент `img` с параметром `data-render-src="http://webpage-url"` и укажите URL-адрес веб-страницы. Отрисовывает моментальный снимок всей веб-страницы на странице OneNote.</p>
[Добавление изображения, созданного из HTML-кода](#add-an-image-rendered-from-html)</p>
Используйте элемент `img` с параметром `data-render-src="name:html-block-name"` и отправьте HTML-код в части данных составного запроса. Отрисовывает HTML в виде изображения на странице OneNote.</p>
[Добавление изображений содержимого PDF-файлов](#add-images-of-pdf-file-contents)</p>
Используйте элемент `<img data-render-src="name:part-name" />` и отправьте PDF-файл в части данных составного запроса. Отрисовывает каждую PDF-страницу в виде отдельного изображения на странице OneNote.</p>
[Добавление файла изображения в качестве вложения](#add-an-image-file-as-an-attachment)</p>
Используйте элемент `object` с параметром `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` и отправьте файл изображения в части данных составного запроса. Добавляет вложенный файл на страницу OneNote и отображает значок файла.</p>

> **Примечание.** Чтобы получить изображения со страницы OneNote, сначала отправьте [запрос GET на получение содержимого страницы](onenote-get-content.md#page-html-content). Будут возвращены URL-адреса ресурсов изображения на странице. Затем разделите [запросы GET на получение ресурсов изображений](onenote-get-content.md#image-or-other-file-resource).


**Атрибуты изображения** 

Элемент **img** при необходимости может включать атрибуты **alt**, **height** и **width**, а также атрибуты стиля **max-width** и **max-height**.

**Типы мультимедиа для изображений**

Microsoft Graph поддерживает типы изображений TIFF, PNG, GIF, JPEG и BMP. Чтобы сохранить изображение другого формата, которое желательно не преобразовывать, [отправьте двоичные данные](#add-an-image-using-binary-data) в составном запросе. Использовать Base64 или другую кодировку для двоичных данных не нужно.

> **Примечание.** API обнаруживает исходный тип входного изображения и возвращает его в виде атрибута **data-fullres-src-type** [выходного HTML-кода](onenote_input_output_html.md#output-html). API также возвращает тип оптимизированного изображения в атрибуте **data-src-type**.
 
Ознакомьтесь с [ограничениями](#size-limitations-for-post-pages-requests) на создание страниц, содержащих файлы мультимедиа.


<a name="image-img-url-src"></a>
### <a name="add-a-public-image-from-the-web"></a>Добавление общедоступного изображения из Интернета

Во входных данных HTML запроса добавьте параметр `<img src="http://..." />` и укажите URL-адрес общедоступного изображения в атрибуте **src**.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Public URL</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image from the web.</p>
    <img src="http://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>
### <a name="add-an-image-using-binary-data"></a>Добавление изображения с помощью двоичных данных

Во входных данных HTML в части **Presentation** запроса добавьте параметр `<img src="name:part-name" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные изображения. Просто отправьте двоичные данные, не используя Base64 или другую кодировку.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Image binary data</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the uploaded image.</p>
    <img src="name:image-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="MyAppPictureId"
Content-Type: image/jpeg

... image binary data ...

--MyAppPartBoundary--  
```


<a name="image-img-url-data-render-src"></a>
### <a name="add-a-webpage-snapshot"></a>Добавление моментального снимка веб-страницы

С помощью Microsoft Graph можно создавать моментальные снимки целых веб-страниц и вставлять их в новые страницы. Этот способ полезен для архивации веб-страниц или сохранения сложных веб-страниц, которые содержат функции, не поддерживаемые приложением OneNote (например, CSS).  

Во входном HTML-коде запроса добавьте параметр `<img src="http://..." />` и укажите URL-адрес нужной веб-страницы в атрибуте **src**.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Webpage capture</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image of the webpage.</p>
    <img data-render-src="http://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>
### <a name="add-an-image-rendered-from-html"></a>Добавление изображения, созданного из HTML-кода
При передаче HTML-кода в виде блока данных убедитесь в отсутствии активного содержимого, для которого могут потребоваться учетные данные пользователя или предварительно загруженный подключаемый модуль браузера. Подсистема, которую Microsoft Graph использует для преобразования HTML-страницы в изображение, не может выполнить вход за пользователя и не включает такие подключаемые модули, как Adobe Flash, Apple QuickTime и т. д. Это также означает, что динамически загружаемое содержимое (например, через скрипт AJAX) не будет отображаться, если для получения данных необходимы учетные данные пользователя или файлы cookie.

Во входных данных HTML в части **Presentation** запроса добавьте параметр `<img data-render-src="name:part-name" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит HTML-код.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: HTML block</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the block of HTML as an image.</p>
    <img data-render-src="name:html-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="html-block-name"
Content-Type: text/html

<html>
<body>
<h1>This HTML will render as an image</h1>
<p><b>Don't</b> try to embed another <i>data-render-src</i> type-image inside the HTML part--
it won't work. Instead, use URL-based real images like this:</p>
<img src="http://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>
### <a name="add-an-image-file-as-an-attachment"></a>Добавление файла изображения в качестве вложения

Во входных данных HTML в части **Presentation** запроса добавьте параметр `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные изображения. Просто отправьте двоичные данные, не используя Base64 или другую кодировку.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Binary image data as file attachment</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page contains the image as a file attachment.</p>
    <object data-attachment="image-file.jpg" data="name:image-block-name" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```

Узнайте больше о [типах файлов мультимедиа](#file-media-types).



<a name="videos"></a>
## <a name="adding-videos"></a>Добавление видео

Вы можете внедрять видео в страницы OneNote с помощью команды `<iframe data-original-src="http://..." />` во входном HTML-коде. 

**Поддерживаемые сайты с видео**

- Dailymotion
- Office Mix
- Sway
- Sketchfab
- TED
- YouTube
- Vimeo
- Vine

**Атрибуты iframe**

**data-original-src**</p>
Обязательный. URL-адрес видео.<br />Пример: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</p>
**width**</p>
Необязательный. Ширина элемента iframe, содержащего видео. Значение по умолчанию: 480.<br />Пример: `width="300"`</p>
**height**</p>
Необязательный. Высота элемента iframe, содержащего видео. Значение по умолчанию: 360.<br />Пример: `height="300"`</p>

**Пример**

Во входном HTML-коде запроса добавьте параметр `<iframe data-original-src="http://..." />` и укажите URL-адрес видео в атрибуте **data-original-src**.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
    <head>
        <title>A page with an embedded video</title>
    </head>
    <body>
        <iframe data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" width="340" height="280"/>
    </body>
</html>

--MyAppPartBoundary--
```


<a name="files"></a>
## <a name="adding-files"></a>Добавление файлов

Вы можете добавлять вложенные файлы в страницы OneNote с помощью элемента **object** во входном HTML-коде. Если вам нужно добавить PDF-файл, вы можете использовать элемент **img** для отрисовки страниц PDF-файла в виде изображений. 

[Добавление вложенного файла](#add-a-file-attachment)</p>
Используйте элемент `<object .../>` и отправьте файл в части данных составного запроса. Добавляет вложенный файл и отображает значок файла на странице OneNote.</p>
[Добавление изображений содержимого PDF-файлов](#add-images-of-pdf-file-contents)</p>
Используйте элемент `<img data-render-src="name:part-name" />` и отправьте PDF-файл в части данных составного запроса. Отрисовывает каждую PDF-страницу в виде отдельного изображения на странице OneNote.</p>

**Атрибуты файлов**

Ниже перечислены обязательные атрибуты элемента **object**.

**data-attachment**</p>
Имя и расширения файла, который нужно отобразить на странице OneNote.<br />Пример: `data-attachment="filename.docx"`</p>
**data**</p>
Имя части body в составном запросе, содержащем двоичные данные файла. Microsoft Graph не поддерживает передачу URL-адресов через этот атрибут.<br />Пример: `data="name:part-name"`</p>
**type**</p>
MIME-тип файла, который используется для определения значка файла для страницы и приложения, запускаемого, когда пользователь активирует файл на устройстве из OneNote.<br />Пример: `type="application/pdf"`</p>


<a name="file-media-types"></a>

### <a name="file-media-types"></a>MIME-типы файлов  
Microsoft Graph использует предопределенный значок для типа вложенного файла или универсальный значок, если API не распознает тип файла. В приведенной ниже таблице показаны распространенные типы файлов, которые распознает этот API.

- application/pdf  
- application/vnd.openxmlformats-officedocument.wordprocessingml.document  
- application/vnd.openxmlformats-officedocument.presentationml.presentation
- application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
- image/png
- image/jpeg
- image/gif
- audio/wav
- video/mp4
- application/msword
- application/mspowerpoint
- application/excel

Ознакомьтесь с [ограничениями](#size-limitations-for-post-pages-requests) на создание страниц, содержащих файлы мультимедиа.


<a name="file-object"></a>
### <a name="add-a-file-attachment"></a>Добавление вложенного файла

Во входных данных HTML в части **Presentation** запроса добавьте параметр `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные файла. Просто отправьте двоичные данные, не используя Base64 или другую кодировку.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image file attachment</title>
  </head>
  <body>
    <p>This is an image file attachment.</p>
    <object data-attachment="Logo.jpg" data="name:logo1-file" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```


<a name="file-binary-data-render-src"></a>
### <a name="add-images-of-pdf-file-contents"></a>Добавление изображений содержимого PDF-файлов

Во входных данных HTML в части **Presentation** запроса добавьте параметр `<img data-render-src="name:part-name" ... />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные файла. Просто отправьте двоичные данные, не используя Base64 или другую кодировку.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with images of the pages of a PDF file</title>
  </head>
  <body>
    <p>The pages of this PDF file render as images.</p>
    <img data-render-src="name:file-part" alt="PDF file as images" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="file-part"
Content-Type: application/pdf

... binary file data ...

--MyAppPartBoundary--  
```


<a name="size-limits"></a>
## <a name="size-limitations-for-post-pages-requests"></a>Ограничения на размер запросов POST для страниц

При отправке изображений и файлов учитывайте следующие ограничения: <!--TODO: check these-->

- Общий максимальный размер данных в запросе POST (включая изображения, файлы и другие данные) составляет приблизительно 70 МБ. Фактическое ограничение зависит от кодировки в нижестоящих системах, поэтому не существует фиксированного ограничения в байтах. Запросы, превышающие это ограничение, могут возвращать ненадежные результаты.

- Ограничение для каждой части данных (включая заголовки) составляет 25 МБ. Microsoft Graph отклоняет части данных, превышающие это ограничение. 

- Максимальное количество изображений на странице составляет 150. При использовании атрибута `src="http://..."` API игнорирует теги **img** после достижения этого предела.

- Каждый запрос POST может включать до 6 частей данных, включая обязательную часть **Presentation**.

- Каждый запрос может содержать до пяти элементов **img** с атрибутом **data-render-src** и один элемент **object** с атрибутом **data-render-src**. Остальные ссылки на изображения и файлы игнорируются.

- Один запрос POST может включать до 30 изображений, независимо от того, какой метод используется для их отправки в API. Остальные изображения игнорируются. Если вам нужно сохранить веб-страницу с большим количеством изображений, рекомендуем [сохранить ее в виде моментального снимка](#add-a-webpage-snapshot).


## <a name="when-to-use-html-versus-data-render-src"></a>Когда использовать HTML, а когда — *data-render-src* 
Если вы выбираете между вставкой HTML на страницу OneNote и использованием атрибута **data-render-src**, учитывайте следующее:

- Сложный HTML, вероятно, лучше отправлять в механизм визуализации с помощью **data-render-src**, а не пытаться изменить HTML так, чтобы его принял Microsoft Graph. Это также относится к тем случаям, когда HTML-код включает неподдерживаемые теги.

- Как правило, точную отрисовку страниц для сохранения макета и внешнего вида страницы лучше обеспечивает механизм визуализации с использованием атрибута **data-render-src**.

- Чтобы текст был доступен для непосредственного редактирования, обычно лучше вставлять HTML-код непосредственно на страницу. Отрисованные изображения сканирует система оптического распознавания символов (OCR), но результаты могут отличаться.

- Моментальный снимок для журнала или архива лучше всего создавать с помощью метода data-render-src.

- Разметка дизайна веб-страницы для централизованного исправления — по-настоящему сильная сторона атрибута **data-render-src**. С помощью возможностей рукописного ввода OneNote вы можете рисовать на изображении, чтобы обозначать изменения или выделять важные части. Сохранение веб-страницы в виде изображения значительно упрощает эту задачу.

- Очень крупные изображения или изображения в форматах, которые OneNote не принимает напрямую, иногда легче преобразовать в эскизы и другие форматы с помощью атрибута **data-render-src**, а не собственного кода. Даже если изображение также доступно в сети, внедрение данных в запрос POST иногда позволяет быстрее сделать сохраненную страницу доступной пользователю OneNote за счет уменьшения общего количества циклов, необходимых для создания страницы OneNote.

Иногда лучший способ определить, какой метод лучше подойдет пользователям — опробовать оба варианта во время разработки приложения.


<a name="permissions"></a>
## <a name="permissions"></a>Разрешения

Для создания и обновления страниц OneNote необходимо запрашивать соответствующие разрешения. Выберите минимальный уровень, необходимый для работы вашего приложения.

**Разрешения для _запросов POST со страницами_**

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All 

**Разрешения для _запросов PATCH со страницами_**

- Notes.ReadWrite
- Notes.ReadWrite.All

Дополнительную информацию о разрешениях и принципе их работы см. в разделе [Разрешения OneNote](permissions_reference.md#notes-permissions).


<a name="see-also"></a>
## <a name="additional-resources"></a>Дополнительные ресурсы

- [Интеграция с OneNote](integrate_with_onenote.md)
- [Блог разработчиков OneNote](http://go.microsoft.com/fwlink/?LinkID=390183)
- [Вопросы о разработке OneNote на сайте Stack Overflow](http://go.microsoft.com/fwlink/?LinkID=390182)
- [Репозитории GitHub OneNote](http://go.microsoft.com/fwlink/?LinkID=390178)  
