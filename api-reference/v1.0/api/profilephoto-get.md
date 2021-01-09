---
title: Получение фотографии
description: Получение указанного объекта profilePhoto или его метаданных (свойств profilePhoto).
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c3bd5a0d69ab392fc55ac1f44bfbe3dc6d74ad08
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790617"
---
# <a name="get-photo"></a>Получение фотографии

Пространство имен: microsoft.graph

Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств profilePhoto).

> **Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).

Поддерживаемые размеры фотографий в формате HD для Microsoft 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648. Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.

Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.
Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.
Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Для ресурса **user**:<br/>User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.Read.All, Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.Read, Contacts.ReadWrite |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается |
|Для приложения                        | Для ресурса **user**:<br/>User.Read.All, User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.Read.All, Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.Read, Contacts.ReadWrite |

> **Примечание.** В настоящее время существует [известная проблема](/graph/known-issues#groups) с доступом к фотографиям группы с помощью разрешений для приложений.

## <a name="http-request"></a>HTTP-запрос

### <a name="get-the-photo"></a>Получение фотографии
<!-- { "blockType": "ignored" } -->

```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```

### <a name="get-the-metadata-of-the-photo"></a>Получение метаданных фотографии
<!-- { "blockType": "ignored" } -->

```http
GET /me/photo
GET /me/photos
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a>Получение метаданных фотографии определенного размера
<!-- { "blockType": "ignored" } -->

```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a>Параметры пути

|Параметр|Тип|Описание|
|:-----|:-----|:-----|
|size  |String  | Размер фотографии. Поддерживаемые размеры фотографий в формате HD для Microsoft 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648. Фотографии могут быть любого размера, если они хранятся в Azure Active Directory. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
### <a name="response-for-getting-the-photo"></a>Отклик для запроса на получение фотографии
При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.
### <a name="response-for-getting-the-metadata-of-the-photo"></a>Отклик для запроса на получение метаданных фотографии
При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.
## <a name="examples"></a>Примеры

### <a name="example-1-get-the-photo-for-the-signed-in-user-in-the-largest-available-size"></a>Пример 1. Получение фотографии пользователя, вошедшего в систему, с максимальным доступным размером
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response"></a>Отклик
Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a>Пример 2. Получение фотографии 48 x 48 для вошедшего пользователя
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a>Отклик
Содержит двоичные данные запрошенной фотографии 48 x 48. Код HTTP-отклика: 200.

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a>Пример 3. Получение метаданных фотографии вошедшего пользователя
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response"></a>Отклик

В данных указанного ниже отклика содержатся метаданные фотографии.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```

## <a name="using-the-binary-data-of-the-requested-photo"></a>Использование двоичных данных запрошенной фотографии

Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты. Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).

```java
const attachments = [{
  '@odata.type': '#microsoft.graph.fileAttachment',
  ContentBytes: file.toString('base64'),
  Name: 'mypic.jpg'
}];
```

Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).

Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения. Ниже приведен пример кода JavaScript для этой операции.

```javascript
const url = window.URL || window.webkitURL;
const blobUrl = url.createObjectURL(image.data);
document.getElementById(imageElement).setAttribute("src", blobUrl);
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

