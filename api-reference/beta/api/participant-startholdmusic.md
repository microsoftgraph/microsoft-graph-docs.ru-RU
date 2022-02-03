---
title: 'участник: startHoldMusic'
description: Приодержите участника и сыграйте музыку в фоновом режиме.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f2319249215f4a2018b5a161154ee27fb9f68d21
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348502"
---
# <a name="participant-startholdmusic"></a>участник: startHoldMusic

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Приодержите](../resources/participant.md) участника и сыграйте музыку в фоновом режиме.
 
> **Примечание:** Только один участник может быть помещен на удержание в любой момент времени.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.                               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                               |
| Приложение                            | Нет. |

> **Примечание:** Проверка разрешений происходит, когда приложение присоединяется или пытается запустить вызов. Дополнительные проверки разрешений не выполняются при запросе `startHoldMusic` .

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/{id}/startHoldMusic
```

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр      | Тип    |Описание|
|:---------------|:--------|:----------|
|customPrompt|microsoft.graph.mediaPrompt|Необязательный параметр. Звуковой запрос, который участник услышит при размещении на удержании.|
|clientContext|String|Необязательный параметр. Уникальная строка контекста клиента. Может иметь не более 256 символов.|

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `202 Accepted` отклика и [объект startHoldMusicOperation](../resources/startholdmusicoperation.md) в тексте ответа.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос
Ниже приведен пример запроса.



# <a name="http"></a>[HTTP](#tab/http)
<!-- { 
  "blockType": "request", 
  "name": "participant-startHoldMusic" 
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/participants/fa1e9582-7145-4ca3-bcd8-577f561fcb6e/startHoldMusic
Content-type: application/json

{
  "customPrompt": {
    "@odata.type": "#microsoft.graph.mediaPrompt",
    "mediaInfo": {
      "@odata.type": "#microsoft.graph.mediaInfo",
      "uri": "https://bot.contoso.com/onHold.wav",
    },
  },
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-startholdmusic-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-startholdmusic-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-startholdmusic-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-startholdmusic-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/participant-startholdmusic-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/participant-startholdmusic-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.startHoldMusicOperation" 
} --> 
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.startHoldMusicOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

### <a name="notification-sent-to-the-application-after-the-startholdmusicoperation-finishes"></a>Уведомление, отправленное в приложение после завершения startHoldMusicOperation

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
      "resourceUrl": "communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.startHoldMusicOperation",
        "@odata.id": "communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```
