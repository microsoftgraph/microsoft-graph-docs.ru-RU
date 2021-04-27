---
title: 'вызов: cancelMediaProcessing'
description: Отменяет обработку мультимедиа для выполнения операций playPrompt или recordResponse.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fe6ecbedcb0d66e5261f08eb3a4aee48db25a493
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047667"
---
# <a name="call-cancelmediaprocessing"></a>вызов: cancelMediaProcessing

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отменяет обработку для любых операций мультимедиа в ходе выполнения.

Операции мультимедиа относятся к операциям IVR [playPrompt](./call-playprompt.md) и [recordResponse,](./call-record.md)которые по умолчанию находятся в очереди для обработки в порядке. Метод **cancelMediaProcessing** отменяет все операции, которые находятся в процессе, а также операции, которые находятся в очереди. Например, этот API можно использовать для очистки очереди операции IVR для новой операции мультимедиа. Однако операция **ubscribeToTone** не отменяется, так как она работает независимо от очереди операции.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.                              |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Отсутствуют.                                       |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр      | Тип    | Описание                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| clientContext  | String  | Клиентский контекст.                                            |

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика HTTP и заглавную головку расположения с URI в `200 OK` [commsOperation,](../resources/commsoperation.md) созданный для этого запроса.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.

##### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-cancelmediaprocessing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.cancelMediaProcessingOperation",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5"
}
```

##### <a name="notification---operation-canceled-for-recordresponse"></a>Уведомление — отмена операции для recordResponse

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
        "status": "failed",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 400,
          "subcode": 8508,
          "message": "Action failed, the operation was cancelled."
        },
        "recordingLocation": "",
        "recordingAccessToken": "",
        "completionReason": "operationCanceled"
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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


