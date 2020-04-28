---
title: 'участник: пригласить'
description: Приглашение участников в активный вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 14c30d53dca55ce99f80cc206a6d746322887240
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455993"
---
# <a name="participant-invite"></a>участник: пригласить

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Приглашение участников в активный вызов.

Дополнительные сведения об обработке операций можно найти в разделе [коммсоператион](../resources/commsoperation.md).

>**Примечание:** Этот API поддерживается только для вызовов групп.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий)                |
| :-------------- | :--------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается                       |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                       |
| Для приложений     | Calls. Инитиатеграупкаллс. ALL                               |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /communications/calls/{id}/participants/invite
```
> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр      | Тип    |Описание|
|:---------------|:--------|:----------|
|participants|Коллекция [invitationParticipantInfo](../resources/invitationparticipantinfo.md)| Приглашенных участников.|
|Контекст|String|Уникальная строка контекста клиента. Максимальный лимит — 256 символов.|

## <a name="response"></a>Ответ
Если сукксессфул, этот метод возвращает код `200 OK` отклика и заголовок Location с URI для [инвитепартиЦипантсоператион](../resources/inviteparticipantsoperation.md) , созданного для этого запроса. В тексте отклика содержится созданный [инвитепартиЦипантсоператион](../resources/inviteparticipantsoperation.md) .

>**Примечание:** Когда этот API возвращает успешный ответ, все участники получат обновление списка.


## <a name="examples"></a>Примеры
В следующих примерах показано, как вызывать этот API.

> **Примечание:** Объекты ответа могут быть сокращены для удобочитаемости. При фактическом вызове будут возвращены все свойства.

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a>Пример 1: приглашение одного участника на существующий вызов группы

##### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "eec3812a-fdc3-4fb4-825c-a06c9f35414e",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "id": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a>Уведомление о завершении операции

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{ 
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064",
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         }
      }
   ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a>Уведомление — список, обновленный при добавлении участника

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "application":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}

```

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a>Пример 2: Приглашение нескольких участников в существующий вызов групп

> **Note**: существующий вызов группы должен иметь допустимый [чатинфо](../resources/chatInfo.md). В приглашении поддерживается до 5 участников.

##### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-multiple"
}-->

```http
POST /communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "identityProvider": "AAD"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "1e126418-44a0-4a94-a6f8-0efe1ad71acb",
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
   "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e",
   "status":"Running",
   "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
   "resultInfo":null,
   "participants":[
      {
         "endpointType":null,
         "id":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
               "identityProvider":"AAD",
               "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      },
      {
         "endpointType":null,
         "id":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
               "identityProvider":"AAD",
               "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      }
   ]
}

```
##### <a name="notification---operation-completed"></a>Уведомление о завершении операции
```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "truncated": "true",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceUrl": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "participants": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
              }
            }
          },
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
              }
            }
          }
        ],
        "status": "completed",
        "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
        "id": null
      }
    }
  ]
}

```
##### <a name="notification---roster-updated-with-participants-added"></a>Уведомление — список, обновленный при добавлении участников
```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->

```json

{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
     "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceUrl": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
              }
            },
            "endpointType": "default"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
                "mediaType": "audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": null
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
             }
            },
            "endpointType": "default"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "3",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": null
        }
      ]
    }
  ]
}


```

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a>Пример 3: приглашение участников в существующий групповой вызов с заменой существующего однорангового вызова


API-интерфейс INVITE поддерживает только одного участника при замене существующего однорангового вызова. Если в теле запроса указано несколько участников, будет прочитан только первый участник, а остальные участники будут игнорироваться.


> **Примечание:** API-интерфейс INVITE поддерживает только одного участника `replacesCallId` , когда он предоставляется. 
> Сведения об использовании `replacesCallId` для замены существующего однорангового звонка содержатся в разделе [инвитатионпартиЦипантинфо](../resources/invitationparticipantinfo.md).

##### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-existing"
}-->

```http
POST /communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "278405a3-f568-4b3e-b684-009193463064",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "id": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "Participant",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a>Уведомление о завершении операции

``` http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->

```json
{ 
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/278405a3-f568-4b3e-b684-009193463064",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/278405a3-f568-4b3e-b684-009193463064",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"278405a3-f568-4b3e-b684-009193463064"
         }
      }
   ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a>Уведомление — список, обновленный при добавлении участника

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->

```json
{
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/communications/calls/a7ebfb2d-871e-419c-87af-27290b22e8db/participants",
         "resourceUrl":"/communications/calls/a7ebfb2d-871e-419c-87af-27290b22e8db/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}
```

>**Примечание:** С состоянием "завершено" вы можете ожидать получения уведомлений о прекращении и удалении исходного однорангового звонка.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
