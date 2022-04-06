---
title: 'вызов: recordResponse'
description: Запись короткого звукового ответа от вызываемой стороны. Это полезно, если бот хочет захватить голосовой ответ от вызываемого после запроса.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9c23f9d50571d963df6d0f73f952af14d4ee4e14
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607570"
---
# <a name="call-recordresponse"></a>вызов: recordResponse

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись короткого звукового ответа от вызываемой стороны.

Бот может использовать это для захвата голосового ответа от вызываемого после запроса ответа.

Дополнительные сведения об обработке операций см. в [commsOperation](../resources/commsOperation.md)

>**Примечание:** Этот API поддерживается только для [вызовов](../resources/call.md) , инициированных с [помощью serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).

Это действие не предназначено для записи всего вызова. Максимальная продолжительность записи — 2 минуты. Запись не будет сохранена платформой облачных коммуникаций и будет отброшена вскоре после окончания вызова. Бот должен быстро скачать запись после завершения операции записи, используя значение recordingLocation, которое дано в завершенной уведомлении.

>**Примечание:** Вы не можете записывать или иным образом сохранять медиаконтент из звонков или собраний, к которые ваше приложение имеет доступ, или данных, полученных из этого медиаконтента. Убедитесь, что вы соответствуете законам и правилам вашей области в отношении защиты данных и конфиденциальности сообщений. Дополнительные сведения можно узнать из [условий использования](/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается        |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается        |
| Для приложений     | Calls.AccessMedia.All                       |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/recordResponse
POST /communications/calls/{id}/recordResponse
```
> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type| application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр      | Тип    |Описание|
|:---------------|:--------|:----------|
|подсказки|[Коллекция MediaPrompt](../resources/mediaprompt.md) | Подсказки для игры. Максимальный поддерживаемый размер коллекции mediaPrompt — 1.|
|bargeInAllowed|Boolean| Если это так, запрос recordResponse будет вступать в другие существующие запросы записи и записи playprompt в очереди или в настоящее время. По умолчанию = false. |
|initialSilenceTimeoutInSeconds | Int32| Максимальная начальная тишина (тишина пользователя) разрешена с того времени, когда мы начнем операцию записи ответа перед периодиалом и не справимся с операцией. Если мы играем запрос, этот отсвечив начинается после завершения запроса. По умолчанию = 5 секунд, Min = 1 секунда, Max = 120 секунд |
|maxSilenceTimeoutInSeconds|Int32| Максимальное время тишины (паузы) после начала выступления пользователя. По умолчанию = 5 секунд, Min = 1 секунда, Max = 120 секунд.|
|maxRecordDurationInSeconds|Int32| Максимальная продолжительность операции recordResponse перед остановкой записи. По умолчанию = 5 секунд, Min = 1 секунда, Max = 120 секунд.|
|playBeep|Boolean| Если это так, воспроизводит звуковой сигнал, чтобы указать пользователю, что он может начать запись своего сообщения. По умолчанию = true.|
|stopTones|Коллекция строк|Стоп-сигналы, указанные для окончания записи.|
|clientContext|Строка|Уникальная строка Client Context. Максимальное ограничение — 256 шаров.|

> **Примечание:** Максимальное время записи сокращено с 5 минут до 2 минут.

## <a name="response"></a>Отклик
Этот метод возвращает код `200 OK` http-ответа и заглавную ссылку Location с URI в [записьОперацией](../resources/recordoperation.md) , созданной для этого запроса.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a>Пример 1. Запись короткого звукового ответа от вызываемой стороны

##### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-recordResponse"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/recordResponse
Content-Type: application/json
Content-Length: 394

{
  "bargeInAllowed": true,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      }
    }
  ],
  "maxRecordDurationInSeconds": 10,
  "initialSilenceTimeoutInSeconds": 5,
  "maxSilenceTimeoutInSeconds": 2,
  "playBeep": true,
  "stopTones": [ "#", "1", "*" ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-recordresponse-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/call-recordresponse-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/call-recordresponse-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже показан пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a>Уведомление — операция завершена

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
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed",
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

### <a name="example-2-retrieving-the-recording-file"></a>Пример 2. Ирисовка файла записи

> **Примечание:** Вы не можете записывать или иным образом сохранять медиаконтент из звонков или собраний, к которые ваше приложение имеет доступ, или данных, полученных из этого медиаконтента. Убедитесь, что вы соответствуете законам и правилам вашей области в отношении защиты данных и конфиденциальности сообщений. Дополнительные сведения можно узнать из [условий использования](/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a>Отклик

<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Transfer-Encoding: chunked
Date: Thu, 17 Jan 2019 01:46:37 GMT
Content-Type: application/octet-stream

(application/octet-stream of size 160696 bytes)
```

> **Примечание:** Вы не можете записывать или иным образом сохранять медиаконтент из звонков или собраний, к которые ваше приложение имеет доступ, или данных, полученных из этого медиаконтента. Убедитесь, что вы соответствуете законам и правилам вашей области в отношении защиты данных и конфиденциальности сообщений. Дополнительные сведения можно узнать из [условий использования](/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: recordResponse",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
