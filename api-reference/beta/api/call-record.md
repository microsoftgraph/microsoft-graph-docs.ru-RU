---
title: 'Call: Record'
description: Запись короткого аудиоклипа из вызова. Это полезно, если пользователь-Робот хочет записать голосовой ответ от абонента, вызываемого после приглашения.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2961bacfa9092aa580801e42e44aa1d2adbfaa97
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636703"
---
# <a name="call-record"></a>Call: Record

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись короткого аудиоклипа из вызова.
С помощью Bot можно получить голосовой ответ от вызывающего абонента после того, как им будет предложено ответить.

Дополнительные сведения о том, как обрабатывать операции, смотрите в [коммсоператион](../resources/commsOperation.md)

>**Примечание:** Это поддерживается только для [вызовов](../resources/call.md) , которые инициируются с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).

Это действие не предназначено для записи всего вызова. Максимальная длина записи составляет 5 минут. Запись не сохраняется окончательно при помощи платформы Cloud Communications и удаляется вскоре после завершения вызова. Bot должен сразу скачать запись после завершения операции записи, используя значение Рекординглокатион, указанное в завершенном уведомлении.

>**Примечание:** Собранные файлы мультимедиа могут быть **не** сохранены. Убедитесь, что вы соответствуете законам и нормативам вашей области, когда дело доходит до записи звонков. Для получения дополнительных сведений обратитесь в юридическое Юрисконсульта.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается        |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается        |
| Приложение     | Calls.AccessMedia.All                       |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /communications/calls/{id}/record
```
> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр      | Тип    |Описание|
|:---------------|:--------|:----------|
|выдан|Коллекция [медиапромпт](../resources/mediaprompt.md) | Коллекция приглашений для воспроизведения (при наличии) до начала записи. Пользователи могут указать действие "Плайпромпт" отдельно или указать его как часть "запись", в основном все записи прецеедед по приглашению. Текущая поддержка предназначена только для одного приглашения в коллекции. |
|баржеиналловед|Логический| Если задано значение true, этот запрос будет барже в другие существующие запросы записи и плайпромпт, находящиеся в очереди. Значение по умолчанию = false. |
|инитиалсиленцетимеаутинсекондс | Int32| Максимальное время ожидания (тишины пользователя), разрешенное с момента запуска операции записи до истечения времени ожидания и неудачи операции. При воспроизведении приглашения этот таймер запускается после завершения приглашения. Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд |
|макссиленцетимеаутинсекондс|Int32| Максимально допустимое время тишины (пауза) после начала диктовки пользователя. Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд.|
|максрекорддуратионинсекондс|Int32| Максимальная длительность операции записи перед остановкой записи. Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд.|
|плайбип|Логический| Если этот параметр имеет значение true, воспроизводит звуковой сигнал, указывающий пользователю, что он может начать запись сообщения. Значение по умолчанию = true.|
|стоптонес|Коллекция String|Остановка заданных тонов в конец записи.|
|Контекст|String|Уникальная строка контекста клиента. Максимальный лимит — 256 символов.|

## <a name="response"></a>Отклик
Этот метод возвращает код `200 OK` отклика и заголовок Location с URI для [рекордоператион](../resources/recordoperation.md) , созданного для этого запроса.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.

### <a name="example-1-record-a-short-audio-clip-from-a-call"></a>Пример 1: запись короткого аудиоклипа из вызова

##### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/record
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
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже показан пример ответа.

> **Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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

### <a name="example-2-retrieving-the-recording-file"></a>Пример 2: получение файла записи

> **Примечание:** Несмотря на то, что вы можете получить и обработать запись, **необходимо** удалить ее позже. Невозможно оставить носитель.

##### <a name="request"></a>Запросить

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a>Ответ

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
