---
title: Получение фотографии
description: Получите указанный profilePhoto или метаданных (**profilePhoto** свойства).
ms.openlocfilehash: 6374680e37d409a89b61d3e2244b45ccb29869e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082784"
---
# <a name="get-photo"></a>Получение фотографии

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Получите указанный [profilePhoto](../resources/profilephoto.md) или метаданных (**profilePhoto** свойства).

GET фотографий операция первая попытка получить указанного фотографий с Office 365. Если фотографии не поддерживается в Office 365, API пытается получить фотографии из Azure Active Directory.

Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648. Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.

Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.
Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.
Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.
Если указанный размер недоступен в почтовом ящике пользователя или Azure Active Directory, возвращается размер 1 x 1 и остальные метаданные.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

> **Примечание:** Операцию GET фотографий в бета-версии поддерживает работой, школа или личных учетных записей пользователя. Операцию GET метаданных фотографий тем не менее, поддерживает только пользователя рабочий или школа учетных записей и не личных учетных записей.

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Для ресурса **user**:<br/>User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.Read.All, Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.Read, Contacts.ReadWrite |
|Делегированные (личная учетная запись Майкрософт)  <br /> **Примечание**: операция метаданных не поддерживается. | Для ресурса **user**:<br/>User.Read, User.ReadWrite<br /><br />Для ресурса **contact**:<br />Contacts.Read, Contacts.ReadWrite |
|Для приложений                        | Для ресурса **user**:<br/>User.Read.All, User.ReadWrite.All<br /><br />Для ресурса **group**:<br />Group.Read.All, Group.ReadWrite.All<br /><br />Для ресурса **contact**:<br />Contacts.Read, Contacts.ReadWrite |

## <a name="http-request"></a>HTTP-запрос 

### <a name="get-the-photo"></a>Получение фотографий
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
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a>Получить метаданные для определенного размера фотографии
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
GET /me/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contacts/{id}/photos/{size}
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
```

## <a name="path-parameters"></a>Параметры пути

|**Параметр**|**Тип**|**Описание**|
|:-----|:-----|:-----|
|size  |String  | Размер фотографии. Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648. Фотографии могут быть любого размера, если они хранятся в Azure Active Directory. |

## <a name="optional-query-parameters"></a>Необязательные параметры запроса
Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ
### <a name="response-for-getting-the-photo"></a>Отклик для запроса на получение фотографии
При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.
### <a name="response-for-getting-the-metadata-of-the-photo"></a>Отклик для запроса на получение метаданных фотографии
При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request-1"></a>Запрос 1
Этот запрос возвращает фотографию пользователя, вошедшего в систему, с максимальным доступным размером.

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a>Отклик 1
Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.

##### <a name="request-2"></a>Запрос 2
Этот запрос получает фотографию 48 x 48 для вошедшего пользователя.

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a>Ответ 2
Содержит двоичные данные запрошенной фотографии 48 x 48. Код HTTP-ответа: 200.

##### <a name="request-3"></a>Запрос 3
Этот запрос возвращает метаданные фотографии вошедшего пользователя.

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a>Ответ 3
В данных указанного ниже ответа содержатся метаданные фотографии. Примечание. Показанный здесь объект ответа может быть усечен для краткости.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена. Примечание. Показанный здесь объект отклика может быть усечен для краткости.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a>Использование двоичных данных запрошенной фотографии

Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты. Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).

Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения. Ниже приведен пример кода JavaScript для этой операции.

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
