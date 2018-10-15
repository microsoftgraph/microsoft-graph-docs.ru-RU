---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
ms.openlocfilehash: c68289049503e70e04b2e403ca09cfc1f67e4096
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268734"
---
# <a name="send-a-sharing-invitation"></a>Отправка приглашения к общему доступу

Отправка приглашения к общему доступу для **DriveItem**.
Приглашение к общему доступу предоставляет получателям разрешения и при необходимости отправляет сообщения электронной почты со [ссылкой общего доступа][].

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

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
| message          | String                         | Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.
| requireSignIn    | Boolean                        | Указывает, должен ли получатель приглашения войти в систему, чтобы просмотреть элемент, к которому предоставлен общий доступ.
| sendInvitation   | Boolean                        | Если значение true, [ссылка общего доступа][] отправляется получателю. В противном случае разрешение предоставляется напрямую без отправки уведомления.
| roles            | Collection(String)             | Указывает роли, которые необходимо предоставить получателям приглашения к общему доступу.

## <a name="example"></a>Пример

В этом примере показано, как отправить приглашение к общему доступу пользователю с электронным адресом "ryan@contoso.org" и добавить сообщение о файле, над которым ведется совместная работа.
Приглашение предоставляет пользователю Райану доступ к файлу на чтение и запись.

### <a name="http-request"></a>HTTP-запрос

При успешном выполнении этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в теле отклика.

<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
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
  "roles": [ "write" ]
}
```

### <a name="response"></a>Ответ

Ниже приведен пример отклика.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a>Замечания

* [Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.
* Список доступных ролей см. в разделе [Перечисление ролей](../resources/permission.md#roles-enumeration).

## <a name="error-responses"></a>Отклики с ошибками

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Отклики с ошибками][error-response].


[DriveRecipient]: ../resources/driverecipient.md
[error-response]: ../../../concepts/errors.md
[ссылка общего доступа]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
