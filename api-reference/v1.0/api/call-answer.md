---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d8719a226f05473ee068bac98364ae5ec01eadaa
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183983"
---
# <a name="call-answer"></a>вызов: ответ

Пространство имен: microsoft.graph

Разрешить интерфейсу Bot ответить на входящий [вызов](../resources/call.md). Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова. При получении приглашения на вызов группы в уведомлении будут содержаться параметры [чатинфо](../resources/chatinfo.md) и [митингинфо](../resources/meetinginfo.md) .

Ожидается, что Bot отвечает, [отклоняется](./call-reject.md)или [перенаправляется](./call-redirect.md) вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.

## <a name="permissions"></a>Permissions
Для ответа на одноранговый звонок не требуется никаких разрешений. Для присоединения к группе необходимо одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий)                 |
| :-------------- | :-----------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается                        |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                        |
| Приложение     | Calls. Жоинграупкаллс. ALL или Calls. Жоинграупкаллсасгуест. ALL |

> **Примечание:** Для вызова, использующего носитель с размещением приложений, вам также потребуется разрешение Calls. Акцессмедиа. ALL. Необходимо иметь по крайней мере одно из следующих разрешений, чтобы обеспечить `source` расшифровку уведомления о входящем вызове: Calls. акцессмедиа. ALL, Calls.Iniтиате. ALL, Calls.IniТиатеграупкалл. ALL, Calls. Жоинграупкалл. ALL, Calls. Жоинграупкалласгуест. ALL. `source`Сведения о вызывающем абоненте в уведомлении о входящем звонке. Без по крайней мере одного из этих разрешений оно `source` останется зашифрованным.

## <a name="http-request"></a>HTTP-запрос
<!-- {"blockType": "ignored" } -->
```http
POST /communications/calls/{id}/answer
```

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр        | Тип                                     |Описание                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|callbackUri       |String                                    |Позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления в дальнейшем. Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot. Это должно быть `https` .    |
|акцептедмодалитиес|Коллекция строк                         |Список принимаемых модальности. Возможные значения: `audio`, `video`, `videoBasedScreenSharing`. Необходимо для ответа на вызов. |
|mediaConfig       | [appHostedMediaConfig](../resources/apphostedmediaconfig.md) или [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md) |Настройка мультимедиа. Потребоваться                                                                                                            |

## <a name="response"></a>Отклик
Этот метод возвращает `202 Accepted` код отклика.

## <a name="examples"></a>Примеры
В приведенном ниже примере показано, как вызывать этот API.

##### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>"
  },
  "acceptedModalities": [
    "audio"
  ]
}
```
Этот большой двоичный объект является сериализованной конфигурацией для сеансов мультимедиа, которая создается из пакета SDK для Media.

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a>Пример 1: ответ одноранговый звонок VoIP с размещенными в службе носителями

##### <a name="notification---incoming"></a>Уведомление — входящий

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
      "changeType": "created",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            }
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a>Запросить

<!-- {
  "blockType": "request",
  "name": "call-answer-service-hosted-media"
}-->
```http
POST /communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a>Ответ
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a>Установка уведомления

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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a>Установленное уведомление

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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a>Пример 2: ответ на звонок VOIP с размещенными в приложении носителями

##### <a name="notification---incoming"></a>Уведомление — входящий

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
      "changeType": "created",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            }
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer-app-hosted-media"
}-->
```http
POST /communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a>Установка уведомления

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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a>Установленное уведомление

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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="example-3-answer-a-policy-based-recording-call"></a>Пример 3: ответ на вызов записи на основе политики

В [сценарии записи на основе политик](https://docs.microsoft.com/microsoftteams/teams-recording-policy), прежде чем участник политики присоединяется к вызову, на Bot, связанном с политикой, будет отправлено уведомление о входящем звонке.
Сведения о присоединении можно найти в свойстве **ботдата** . С помощью Bot можно выбрать ответ на вызов и соответствующим образом [Обновить состояние записи](call-updaterecordingstatus.md) .

Ниже приведен пример уведомления о входящем вызове, которое будет получено в этом случае.

```json
{
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"created",
         "resource":"/app/calls/e71f0300-9c1f-4d99-b5f4-2722e877d497",
         "resourceUrl":"/communications/calls/e71f0300-9c1f-4d99-b5f4-2722e877d497",
         "resourceData":{
            "@odata.type":"#microsoft.graph.call",
            "state":"incoming",
            "direction":"incoming",
            "source":{
               "@odata.type":"#microsoft.graph.participantInfo",
               "id":"90fad2ce-8989-41a1-8a66-f6636e629a2a",
               "identity":{
                  "@odata.type":"#microsoft.graph.identitySet",
                  "user":{
                     "@odata.type":"#microsoft.graph.identity",
                     "id":"8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
                     "identityProvider":"AAD"
                  }
               },
               "endpointType":"default",
               "region":"amer"
            },
            "targets":[
               {
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "applicationInstance":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"832899f8-2ea1-4604-8413-27bd2892079f",
                        "identityProvider":"AAD"
                     }
                  },
                  "endpointType":"default",
                  "id":"4520a1a5-5394-5a41-aa12-9ee6fa18cfc8",
                  "region":null,
                  "languageId":null
               }
            ],
            "meetingInfo":{
               "@odata.type":"#microsoft.graph.tokenMeetingInfo",
               "token":"join token"
            },
            "tenantId":"932899f8-2ea1-4604-8413-27bd2892079f",
            "myParticipantId":"1520a1a5-5394-4a41-aa72-9ee6fa18cfc8",
            "callChainId":"05f2f70f-3a9c-47c1-80a9-cc79e91d8cec",
            "incomingContext":{
               "@odata.type":"#microsoft.graph.incomingContext",
               "sourceParticipantId":"30fad2ce-8989-41a1-8a66-f6636e629a2a",
               "observedParticipantId":"30fad2ce-8989-41a1-8a66-f6636e629a2a"
            },
            "id":"e71f0300-9c1f-4d99-b5f4-2722e877d497",
            "applicationMetadata":{
               "botData":{
                  "mediaHostedRegion":"USEA",
                  "user":{
                     "participationMethod":"callee",
                     "clientLocation":"US"
                  },
                  "otherSideUser":{
                     "id":"971f0300-9c1f-4d99-b5f4-2722e877d490",
                     "participantId":"3520a1a5-5394-4a41-aa72-9ee6fa18cfc8",
                     "tenantId":"1540a1a5-2394-4a41-aa72-9ee6fa18cfc8",
                     "onBehalfOf":{
                        "id":"871f0300-9c1f-4d99-b5f4-2722e877d490"
                     },
                     "participationMethod":"caller",
                     "clientLocation":"EUNO"
                  },
                  "inviteReasons":[
                     "PolicyBasedRecording"
                  ],
                  "policyIdentifier":"Test Policy",
                  "pairedRecorders":[
                     {
                        "id":"471f0300-5c1f-4d99-b5f4-2722e877d490",
                        "participantId":"371f0300-2c1f-4d99-b5f4-2722e877d490"
                     }
                  ],
                  "otherRecorders":[
                     {
                        "id":"671f0300-9c1f-4d99-b5f4-2722e877d490",
                        "participantId":"a71f0300-ec1f-4d99-b5f4-2722e877d490"
                     }
                  ]
               }
            }
         }
      }
   ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
