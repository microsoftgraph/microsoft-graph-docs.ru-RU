---
title: Создание страницы
description: Создайте новую страницу OneNote в разделе по умолчанию записной книжки по умолчанию.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 828fc09e3b7cdb281b682df93b3d6f94f264330d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004643"
---
# <a name="create-page"></a>Создание страницы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новую страницу OneNote в разделе по умолчанию записной книжки по умолчанию.

Чтобы создать страницу в другом разделе записной книжки, используемой по умолчанию, можно использовать `sectionName` параметр запроса.  Пример: `../onenote/pages?sectionName=My%20section`.

Эта `POST /onenote/pages` операция используется только для создания страниц в записной книжке текущего пользователя по умолчанию. Если вы нацелены на другие записные книжки, вы можете [создавать страницы в указанном разделе](../api/section-post-pages.md).      

> **Примечание:** Существует предельное число страниц, которые можно добавить в раздел с помощью этого API. Дополнительные сведения см. в статье [Создание страниц OneNote](/graph/onenote-create-page) для всех ограничений с помощью этого API.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Notes.Create, Notes.ReadWrite    |
|Для приложений | Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a>Заголовки запросов  
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type | string | `text/html` или `application/xhtml+xml` для содержимого HTML, в том числе для необходимой части Presentation составных запросов. В составных запросах используется тип содержимого `multipart/form-data; boundary=your-boundary`. |

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте HTML-контент для страницы.

Текст может содержать HTML-код, размещенный прямо в тексте запроса, либо формат составного сообщения, как показано в примере. Если вы отправляете двоичные данные, необходимо отправить составной запрос.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [оненотепаже](../resources/onenotepage.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

В `../onenote/pages` пути можно использовать `sectionName` параметр запроса, чтобы создать страницу в определенном разделе записной книжки по умолчанию. Пример: `../onenote/pages?sectionName=My%20section`. Если раздел не существует (или был переименован), API создаст новый раздел.

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages
Content-length: 312
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
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
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


