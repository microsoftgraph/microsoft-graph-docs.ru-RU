---
title: 'call: addLargeGalleryView'
description: Добавьте представление большой коллекции в вызов.
author: navali-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 41420667a36d81c14b5e6bf5dd13b8ee274872f1
ms.sourcegitcommit: 4ff6e89e89178cbd5aef8aa019e714d95817fae4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2022
ms.locfileid: "65017059"
---
# <a name="call-addlargegalleryview"></a>call: addLargeGalleryView

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте представление большой коллекции в вызов.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.       |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.       |
| Приложение     | Calls.JoinGroupCallAsGuest.All, Calls.JoinGroupCall.All, Calls.InitiateGroupCall.All                       |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/addLargeGalleryView
POST /communications/calls/{id}/addLargeGalleryView
```

> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание                |
|:--------------|:---------------------------|
| Авторизация | Bearer {token}. Обязательный.  |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите объект JSON со следующим параметром.

| Параметр      | Тип    | Описание |
|:---------------|:--------|:------------|
| clientContext  | String  | Уникальная строка контекста клиента, которая может содержать не более 256 символов. |

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `202 Accepted` отклика и объект [addLargeGalleryViewOperation](../resources/addlargegalleryviewoperation.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В следующем примере показано, как добавить представление большой коллекции в вызов.

<!-- {
  "blockType": "request",
  "name": "addLargeGalleryView-1"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/addLargeGalleryView
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "785f4929-92ca-497b-863f-c778c77c9758"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "addLargeGalleryView-1",
  "truncated": true,
  "@odata.type": "microsoft.graph.addLargeGalleryViewOperation"
} -->
```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/e33176d4-836a-4fd7-b95a-d11bda52811d

{
  "@odata.type": "#microsoft.graph.addLargeGalleryViewOperation",
  "clientContext": "785f4929-92ca-497b-863f-c778c77c9758",
  "id": "e33176d4-836a-4fd7-b95a-d11bda52811d",
  "resultInfo": null,
  "status": "running"
}
```

### <a name="notification---operation-completed"></a>Уведомление — операция завершена

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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/e33176d4-836a-4fd7-b95a-d11bda52811d",
      "resourceData": {
        "@odata.type": "#microsoft.graph.addLargeGalleryViewOperation",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/e33176d4-836a-4fd7-b95a-d11bda52811d",
        "clientContext": "785f4929-92ca-497b-863f-c778c77c9758",
        "status": "completed"
      }
    }
  ]
}
```

## <a name="see-also"></a>См. также

- [Узнайте, как определить участника представления большой коллекции в вызове](/graph/cloud-communications-identifylargegalleryview)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: addLargeGalleryView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
