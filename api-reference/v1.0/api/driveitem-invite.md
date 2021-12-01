---
author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения для доступа к элементу
ms.localizationpriority: medium
ms.prod: sharepoint
description: Отправляет приглашение общего доступа для driveItem.
doc_type: apiPageType
ms.openlocfilehash: 0ce6f6751d206571a2d55f31e6e90fcb635df4c2
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61241283"
---
# <a name="send-a-sharing-invitation"></a>Отправка приглашения к совместному использованию

Пространство имен: microsoft.graph

Отправляет приглашение общего доступа для **driveItem.**
Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им сообщение электронной почты с [ссылкой совместного доступа][].

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| Параметр        | Тип                           | Описание
|:-----------------|:-------------------------------|:-------------------------
| recipients       | Collection([DriveRecipient][]) | Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.
| message          | String                         | Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.
| requireSignIn    | Boolean                        | Указывает, должен ли получатель приглашения выполнить вход, чтобы просмотреть элемент, к которому предоставлен общий доступ.
| sendInvitation   | Boolean                        | Если указано значение true, получателю отправляется [ссылка совместного доступа][]. В противном случае разрешение предоставляется напрямую без отправки уведомления.
| roles            | Collection(String)             | Указывает роли, которые необходимо предоставить получателям приглашения к совместному использованию.
| expirationDateTime | DateTimeOffset                       | Укажите dateTime, по истечении которого истекает срок действия разрешения. Доступно на OneDrive для бизнеса, SharePoint и премиум-OneDrive учетных записей.
| password           | Строка                         | Пароль, установленный на приглашении создателем. Необязательный и OneDrive только личный.

## <a name="example"></a>Пример

В этом примере показано, как отправить приглашение к совместному использованию пользователю с электронным адресом ryan@contoso.com и добавить сообщение о файле, над которым ведется совместная работа. Приглашение предоставляет Райану доступ к файлу для чтения и записи.

### <a name="http-request"></a>HTTP-запрос

При успешном выполнении этот метод возвращает код ответа `200 OK` и объект коллекции [permission](../resources/permission.md) в теле ответа.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@deprecated.GrantedTo": "GrantedTo has been deprecated. Refer to GrantedToV2",
      "grantedTo": {
        "user": {
          "displayName": "Robin Danielsen",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "grantedToV2": {
        "user": {
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20",
          "displayName": "Robin Danielsen"
        },
        "siteUser": {
          "id": "1",
          "displayName": "Robin Danielsen",
          "loginName": "Robin Danielsen"
        }
      },
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "robin@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```

## <a name="remarks"></a>Примечания

* [Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.
* Список доступных ролей см. в списке [значений свойств ролей.](../resources/permission.md#roles-property-values)

## <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Отклики ошибок][error-response].


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[ссылка совместного доступа]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
} -->

