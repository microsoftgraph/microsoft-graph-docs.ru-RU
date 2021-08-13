---
title: Создание страниц OneNote
description: " Корпоративная записная книжка в Microsoft 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 4bfd49759e7503992592492b17775e1d7ffb54015434dcca4a628afc0779550b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165576"
---
# <a name="create-onenote-pages"></a>Создание страниц OneNote

**Область применения:** Пользовательские записные книжки в OneDrive | Корпоративные записные книжки в Microsoft 365.

Чтобы создать страницу OneNote, отправьте запрос POST в конечную точку *pages*. Пример:

`POST ../notes/sections/{id}/pages`

<br/>

Отправьте в тексте сообщения HTML-код, определяющий страницу. Если запрос выполнен успешно, Microsoft Graph возвращает код состояния HTTP 201.


> **Примечание.** Сведения о запросах POST, которые вы можете отправлять для создания разделов, групп разделов и записных книжек, см. в [интерактивном справочнике по REST](https://dev.onenote.com/docs).


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>Создание URI запроса

Чтобы создать URI запроса POST, начните с корневого URL-адреса службы:

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

Затем добавьте конечную точку *pages*:

- **Создание страницы в любом разделе (по его названию)**<br/><br/>`.../pages?sectionName=DefaultSection`

- **Создание страницы в любом разделе (по его идентификатору)**<br/><br/>`.../sections/{section-id}/pages` 

При создании страниц в личной записной книжке пользователя Microsoft Graph также предоставляет конечные точки, с помощью которых можно создавать страницы в записной книжке по умолчанию:

- **Создание страницы в стандартном разделе стандартной записной книжки**<br/><br/>`../pages` 



Полный URI запроса будет выглядеть так, как в одном из следующих примеров:

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

См. дополнительные сведения о [корневом URL-адресе службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a>Использование параметра *sectionName* URL-адреса

При создании страницы в именованном разделе записной книжки по умолчанию с помощью параметра *sectionName* действуют следующие правила:

- Можно ссылаться только на разделы верхнего уровня (не внутри групп разделов).

- Если в стандартной записной книжке нет раздела с указанным названием, API создает его. В названиях разделов не допускаются следующие символы: `? * \ / : < > | & # " % ~`

- При сопоставлении названий разделов регистр не учитывается, но он сохраняется при их создании. Например, если указать название "Мой новый раздел", то оно будет отображаться и дальше, но в последующих запросах можно использовать имя "мой новый раздел".

- В названиях разделов следует использовать кодировку URL. Например, пробелы следует кодировать как *%20*.

- Параметр *sectionName* действителен только с маршрутом `../notes/pages` (не `../notes/sections/{id}/pages`).

Разделы создаются только в случае их отсутствия, поэтому этот вызов можно использовать для каждой страницы, создаваемой приложением. Пользователи могут переименовывать разделы, но при этом API создаст новый раздел с указанным вами названием. 

> **Примечание.** Возвращаемые интерфейсом API ссылки на страницы в переименованном разделе по-прежнему будут указывать на старые страницы. 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>Составление текста сообщения

HTML-код, определяющий содержимое страницы, называют *входным HTML-кодом*. Входной HTML-код поддерживает [часть стандартных атрибутов HTML и CSS](#supported-html-and-css-for-onenote-pages), а также настраиваемые атрибуты. (Настраиваемые атрибуты, например **data-id** и **data-render-src**, описываются в статье [Входной и выходной HTML-код](onenote-input-output-html.md).) 

Отправьте входной HTML-код в тексте сообщения запроса POST. Вы можете отправить HTML-код прямо в тексте сообщения, используя тип контента `application/xhtml+xml` или `text/html`, или в части Presentation составного запроса. 

В приведенном ниже примере входной HTML-код отправляется прямо в тексте сообщения.

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="https://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

Если вы отправляете двоичные данные, необходимо использовать [составной запрос](#example-request). 

> **Примечание.** Чтобы упростить программирование и обеспечение согласованности в приложении, вы можете использовать составные запросы для создания всех страниц. Рекомендуем использовать библиотеку для создания составных сообщений. Это снижает риск создания полезных данных в неправильном формате.


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a>Требования и ограничения для входного HTML-кода в запросах POST для страниц

Отправляя входной HTML-код, учитывайте следующие требования и ограничения:  

- Входной HTML-код должен быть правильно оформленным XHTML-кодом с кодировкой UTF-8. Всем открывающим тегам контейнеров должны соответствовать закрывающие теги. Все значения атрибутов должны быть заключены в двойные или одинарные кавычки.  <!--docs say MUST be encoded-->

- Код JavaScript, вложенные файлы и CSS удаляются. 

- HTML-формы полностью удаляются.  

- Microsoft Graph поддерживает [подмножество элементов HTML](#supported-html-and-css-for-onenote-pages). 

- Microsoft Graph поддерживает отдельные стандартные атрибуты HTML и ряд настраиваемых атрибутов, таких как атрибут **data-id**, используемый для обновления страниц. Поддерживаемые атрибуты описываются в статье [Входной и выходной HTML-код](onenote-input-output-html.md).


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a>Поддерживаемые атрибуты HTML и CSS для страниц OneNote

Поддерживаются не все элементы, атрибуты и свойства (в HTML4, XHTML, CSS, HTML5 и т. д). Microsoft Graph принимает ограниченный набор элементов HTML, более соответствующий особенностям работы с OneNote. Дополнительные сведения см. на странице [Поддержка HTML-тегов для страниц](https://dev.onenote.com/docs#/introduction/html-tag-support-for-pages). Если тег не указан на этой странице, скорее всего, он будет игнорироваться.

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

Ниже перечислены базовые типы элементов, которые поддерживает Microsoft Graph:

- `<head>` и `<body>`</p>
- `<title>` и `<meta>`, которые задают заголовок и дату создания страницы</p>
- `<h1>` — `<h6>` для заголовков разделов</p>
- `<p>` для абзацев</p>
- `<ul>`, `<ol>` и `<li>` для списков и их элементов</p>
- `<table>`, `<tr>` и `<td>`, включая вложенные таблицы</p>
- `<pre>` для предварительно отформатированного текста (с сохранением пробелов и разрывов строк)</p>
- `<b>` и `<i>` для полужирного текста и курсива</p>

Microsoft Graph сохраняет семантическое содержимое и базовую структуру входного HTML-кода при создании страниц, но преобразует входной HTML-код для использования поддерживаемого набора элементов HTML и CSS. Функции, отсутствующие в OneNote, преобразовывать не во что, поэтому они могут не распознаваться в исходном HTML-коде. 


<a name="example"></a>

## <a name="example-request"></a>Пример запроса

Этот пример составного запроса создает страницу, содержащую изображения и внедренный файл. Обязательная часть **Presentation** содержит входной HTML-код, определяющий страницу. Часть **imageBlock1** содержит двоичные данные изображения, а **fileBlock1** — двоичные данные файла. Части данных также могут содержать HTML-код. В этом случае Microsoft Graph [отображает HTML-код в виде изображения](onenote-images-files.md#add-an-image-using-binary-data) на странице OneNote. 

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```

Дополнительные примеры создания страниц, содержащих изображения и другие файлы, см. в статье [Добавление изображений и файлов](onenote-images-files.md), наших [руководствах](/previous-versions/office/office-365-api/how-to/onenote-tutorial) и [примерах](https://github.com/onenotedev). Кроме того, узнайте, как [создавать элементы с абсолютным положением](onenote-abs-pos.md), [использовать теги примечаний](onenote-note-tags.md), а также [извлекать данные](onenote-extract-data.md) из визитных карточек, рецептов из Интернета и описаний товаров.

Microsoft Graph требует строгого соответствия некоторым форматам, таким как символы новой строки CRLF в тексте составного сообщения. Чтобы снизить риск получения полезных данных в неправильном формате, для создания составных сообщений следует использовать библиотеку. 

Если появится состояние 400 (неправильный формат полезных данных), проверьте форматирование символов новой строки и пробелов, а также наличие проблем с кодировкой. Например, попробуйте использовать параметр `charset=utf-8` (пример: `Content-Type: text/html; charset=utf-8`).

См. [требования и ограничения для входного HTML-кода](#requirements-and-limitations-for-input-html-in-post-pages-requests) и [ограничения размера запросов POST](onenote-images-files.md#size-limitations-for-post-pages-requests).


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a>Информация о запросах *POST для страниц* и соответствующих ответах

| Данные запроса | Описание |  
|------|------|  
| Протокол | Все запросы используют протокол SSL/TLS для HTTPS. |  
| Заголовок Authorization | <p>`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</p><p>Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401. См. статью [Проверка подлинности и разрешения](permissions-reference.md).</p> |  
| Заголовок Content-Type | <p>`text/html` или `application/xhtml+xml` для HTML-содержимого, отправляемого либо непосредственно в тексте сообщения, либо в обязательной части Presentation составных запросов.</p><p>Составные запросы необходимы при отправке двоичных данных и используют тип контента `multipart/form-data; boundary=part-boundary`, где `{part-boundary}` — это строка, обозначающая начало и конец каждой части данных.</p> |  
| Заголовок Accept | `application/json` | 

<br/>

| Данные ответа | Описание |  
|------|------|  
| Код успешного завершения | Код состояния HTTP 201 |  
| Текст ответа | Представление OData новой страницы в формате JSON. |  
| Ошибки | Если запрос завершается сбоем, API возвращает ошибки в объекте **\@api.diagnostics** в тексте ответа. |  
| Заголовок Location | URL-адрес ресурса новой страницы. |  
| Заголовок X-CorrelationId | GUID, уникальный идентификатор запроса. Это значение можно использовать вместе со значением заголовка Date при устранении неполадок совместно со службой поддержки Майкрософт. |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>Составление корневого URL-адреса службы Microsoft Graph

В корневом URL-адресе службы Microsoft Graph используется следующий формат для всех вызовов Microsoft Graph:

`https://graph.microsoft.com/{version}/me/onenote/`  

Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph. Используйте значение `v1.0` для стабильного кода в рабочей среде. Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки. Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде. 

Используйте значение `me` для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым). Используйте значение `users/{id}` для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем. Используйте [Microsoft Graph](https://graph.microsoft.com/v1.0/users) для получения идентификаторов пользователей. 

<a name="limitations"></a>

## <a name="onenote-section-size-limitations"></a>Ограничения размера раздела OneNote
Существует ограничение на количество страниц, которые можно добавить в раздел с помощью API OneNote. Когда этот предел достигнут для раздела и предпринята попытка создать новую страницу в этом разделе, вы увидите ответ с кодом состояния HTTP `507` и сообщением «Превышено максимально допустимое количество страниц в разделе». Дополнительные сведения об этом коде ошибки см. В разделе [Коды ошибок OneNote](onenote-error-codes.md).

Вы можете использовать один из следующих обходных путей:
- Создайте новый раздел и добавьте туда новые страницы.
- Удалите неиспользуемые страницы из существующего раздела, который достиг ограничения страницы.

<a name="permissions"></a>

## <a name="permissions"></a>Permissions

Для создания страниц OneNote необходимо запрашивать соответствующие разрешения. Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.

Варианты:

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All

Дополнительные сведения об областях разрешений и принципе их использования см. в [справочнике по разрешениям Microsoft Graph](permissions-reference.md).




<a name="see-also"></a>

## <a name="see-also"></a>См. также

- [Добавление изображений и файлов](onenote-images-files.md)
- [Создание элементов с абсолютным положением](onenote-abs-pos.md)  
- [Извлечение данных](onenote-extract-data.md)
- [Использование тегов заметок](onenote-note-tags.md)
- [Интеграция с OneNote](integrate-with-onenote.md)
- [Блог разработчиков OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»](/answers/topics/microsoft-graph-notes.html)
- [Репозитории GitHub OneNote](https://go.microsoft.com/fwlink/?LinkID=390178)